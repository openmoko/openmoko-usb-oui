Open registry for community / homebrew USB Product IDs + OUI
============================================================

**Do not apply before your project is published under a FOSS license!**

As the openmoko products have been discontinued, Openmoko Inc. has been
opening up the use of its *USB Vendor ID* and *IEEE OUI* for use by the
Free and Open Source software and hardware communities. This means you
can simply register your devices and will get an allocation of a Product
ID for free.

**Do not apply before your project is published under a FOSS license!**

Conditions
----------

**Do not apply before your project is published under a FOSS license!**

By applying for an Openmoko Product ID, you acknowledge that either

* the USB device you are developing is an open hardware project
  (as per the [OSHW Definition](http://www.oshwa.org/definition/)), or
* the firmware/software running on your USB device is Free / Open Source
  software, licensed under an OSI-Approved, FSF-Recognized or
  DFSG-Approved Free / Open Source software license

**Do not apply before your project is published under a FOSS license!**

How to Apply for an USB PID or IEEE OUI sub-range
-------------------------------------------------

In order to request a product ID, please send an pull-request to the
[openmoko-usb-oui](https://github.com/openmoko/openmoko-usb-oui) github
project.

Please make sure the commit log message of your pull requests contains
the following details:

* the string "request" somewhere in the subject
* a name and short description of your USB device project
* the license under which you are releasing the hardware and/or software/firmware of the device
* a link to the project website and/or source code repository, if any
* a terse descriptive string for each ID you want, according to the examples below (field#3 in table). This string will show up in tools like `lsusb` etc and should avoid to use "USB" to describe what the device is/does, since those tools are implicitly about USB already. (bad: "USB keyboard", less bad: "Joe's USB-RS232 adapter" (established term in one word), BEST: "ACME1 secure mass storage device, type 512")
* if you (might) need multiple Product IDs, please indicate + explain this at the first message, rather than applying for a second ID later, so we can allocate a contiguous range.

If you do not have a github account, do not wish to use it, or have any other question, you can contact us per email at usb-id AT lists.openmoko.org.

**Do not apply before your project is published under a FOSS license!**

Checklist for a perfect application
-----------------------------------

Here are a couple of aspects you should complete before applying for a USB PID or IEEE OUI.
This is what we will look for before being able to grand you the ID.

Regarding hardware:

1. Have a README[.txt|.md] file describing which part is under which license
    - this will help to quickly identify the project's license, particularly when several licenses are combined, or your are using libraries under other licenses. Also make sure the combination is allowed by the individual licenses.
2. Include all full text licenses in a LICENSE[.txt] file
3. Include a copyright notice in the schematic sheet(s), including author and date
    - this will determine who the copyright holder is, and when the copyright will expire.
4. Include the license name in the schematic sheet(s)
    - this becomes important when different license are combined, and parts of the project, or libraries, are under different licenses
5. Include all schematic symbols and board footprint libraries in the project
    - without that the project can't be seen as complete. Also ensure their license is compatible.
6. Export the schematic capture as pdf, and board layout as gerber+NC drill [and other fabrication output] files
    - not every user can, or wants, to install the EDA suite you are using. This is even more important if in the future this suite stops supporting the current format. If you don't want to mix the fabrication output with the source files, have a general project page pointing to the source files and fabrication output.

Regarding software, firmware, or gateware:

1. Have a README[.txt|.md] file describing which part is under which license
    - this will help to quickly identify the project's license, particularly when several licenses are combined, or your are using libraries under other licenses. Also make sure the combination is allowed by the individual licenses.
2. Include all full text licenses in a LICENSE[.txt] file
3. Ensure the source files have a copyright notice, including author and date
    - this will determine who the copyright holder is, and when the code will become public domain once the copyright expires
4. Ensure the source files have a license header. A SPDX-License-Identifier is sufficient.
    - this becomes important when different license are combined, and parts of the project, or libraries, are under different licenses
5. Don't request a sub-range to include each individual hardware supporting this software. Use one USB PID and include hardware information in the USB description
    - our USB PID range is not infinite, and we would like to be able to continue offering PIDs in the future.
