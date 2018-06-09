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

Please make sure the commitlog message of your pull requests contains
the following details:

* the string "request" somewhere in the subject
* a name and short description of your usb device project
* the license under which you are releasing the hardware and/or software/firmware of the device
* a link to the project website and/or source code repository, if any
* a terse descriptive string for each ID you want, according to the examples below (field#3 in table). This string will show up in tools like `lsusb` etc and should avoid to use "USB" to describe what the device is/does, since those tools are implicitly about USB already. (bad: "USB keyboard", less bad: "Joe's USB-RS232 adapter" (established term in one word), BEST: "ACME1 secure mass storage device, type 512")

* if you (might) need multiple Product IDs, please indicate + explain this at the first message, rather than applying for a second ID later, so we can allocate a contiguous range.

Feel free to also contact us on IRC, #openmoko channel on Freenode.

**Do not apply before your project is published under a FOSS license!**
