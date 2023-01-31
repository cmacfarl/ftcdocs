
Scoring Software Event Setup
============================

This is a quick start guide for setting up the event management/scoring
software for an FTC Event.  A more detailed guide for using the software and
running an event may be found in the
`Scorekeeper Guide <https://firstinspiresst01.blob.core.windows.net/first-energize-ftc/scorekeeper-guide.pdf>`_

.. attention:: This document is intended for Event Adminstrators and Event
   Scorekeepers who are setting up a *traditional* FTC event.  Roles can be
   confirmed by going to an Event Dashboard on
   `ftc-scoring <https://ftc-scoring.firstinspires.org>`_ and selecting
   Event Users.  If you do not have one of these roles for an upcoming event,
   or you don't have access to an Event Dashboard, please contact your PDP
   for assistance.

Requirements
------------

The FIRST Tech Challenge Live software is available for the Windows and Mac
platforms. It is a browser-based application, meaning that you interact with
the system exclusively through a web browser. The system supports real-time
score tracking, inspection tracking, head ref notes and FTA notes. Live score
data can be entered into the system using a tablet.

General
^^^^^^^

   - Intel Core i5 Processor
   - 4 GB of RAM
   - 300 MB of available disk space
   - CAT 5 Ethernet adapter to hardwire to router.
   - 802.11 WiFi adapter (optional)
   - Google Chrome version 80 and higher; Firefox is not supported.

Windows
^^^^^^^

   - Windows 10
   - `Java 8 for Windows <https://www.java.com/en/download/>`_ or higher on the laptop running running the FTCLive software

Mac
^^^

   - macOS Sierra or greater
   - `Java 8 for Mac <https://www.java.com/en/download/help/mac_install.html>`_ or higher on the laptop running the FTCLive software

.. caution:: Unlike the Windows environment, macOS **MAY** require the Java
   Development Kit (JDK) to run. Windows only requires the Java Runtime
   Environment (JRE) to run. If you install the JDK software onto your Mac,
   you should not need to install the JRE software. The JRE should already be
   included as part of the JDK

.. warning:: Need confirmation on whether or not mac users need JDK.

Tablets are necessary for live score tracking.  Either Android or Apple tablets
may be used regardless of the operating system of the scoring server.

Android
^^^^^^^

   - Android Marshmallow (6.x) or greater
   - Google Chrome 80 and higher
   - Support for Wi-F

Apple
^^^^^

   - iOS 15 or greater
   - Google Chrome
   - Support for Wi-Fi

Installing FTCLive
------------------

Download the `latest FTCLive release <https://github.com/FIRST-Tech-Challenge/scorekeeper/releases>`_

The software is stored as a compressed archive file and is available in .zip
format. There are a few releases each season so make sure the version for the
event is up-to-date.

.. warning:: Each release incorporates its own local database for the server.
   Therefore, if you install multiple releases in multiple locations it is very
   easy to start the wrong version and then wonder where your events are
   because they are in the database associated with the other version.  To
   avoid this, either delete older versions entirely, which also removes the
   event archives that were run using the older version, or make sure the
   scorekeeper knows there are multiple instances of FTCLive on the machine
   and knows to run the correct version.

Once you have downloaded and unzipped the archive, navigate to the
folder it was unzipped in and either double click the .bat file for Windows,
or -UNIX file for Mac and Linux.

A console window will appear.  The scoring server is running in this
window.  The window may be minimized, but should not be closed.  After a
short period of time, a browser will be launched pointing at the scoring
server's main page.

Setting Up An Event
-------------------

Setting up an event for competition day involves transferring event day
information from `ftc-scoring <https://ftc-scoring.firstinspires.org`_ to
the `FTCLive <https://github.com/FIRST-Tech-Challenge/scorekeeper`_ server
running on the local event scoring server laptop.

The Easy Way
------------

Step 1: Ensure the scoring server is running on the scoring server laptop.
Login to the server using the default username and password shown on the
server's login page.

Step 2: Login to https://ftc-scoring.firstinspires.org , find the event you
are setting up for, navigate to the event's homepage, select Manage Event to
bring up the Event Dashboard, select Play Event Locally.

Step 3: Confirm that ftc-scoring can detect the FTCLive scoring server, and
then select Import This Event.  Confirm the event setup, then click Confirm.

Once you've clicked Confirm on ftc-scoring, the event database is downloaded
to the scoring server laptop and your browser is automatically switched over
to FTCLive and you are ready to run the event.

.. tip:: If teams were added to the event within ftc-scoring, then the
   team list will be present in the downloaded database.  Event Administrators
   or PDPs should populate team lists in ftc-scoring as soon as team lists for
   an event are known.

The Slightly Harder Way
-----------------------

Step 1: Obtain an Event Key from an Event Administrator or PDP.  Event Keys
are available from the Play Event Locally page described above under Manual
Setup on ftc-scoring.

.. note:: Event Keys are not Event Codes, but are often confused for one
   another.  An Event Key is a Universally Unique Identifier
   distinguished by a series of hexadecimal numbers separated by hashes and
   should only be disclosed to Event Administrators or Lead Scorekeepers for
   a particular event.  They should be treated as passwords and kept secure.
   An Event Code is a publicly known unique key that identifies an event.
   There is no secrecy requirement for Event Codes, and in fact they are
   commonly used in url paths.

Step 2: On the FTCLive server, from the main page select Event Admin -> Setup
Event, enter the Event Key in the text entry box and click Submit.

Best Practices
--------------

   - Do not run the scoring server network over school wi-fi.
   - Disable any firewall, or open appropriate ports, on the computer that will
     be running the server.
   - Disable any ad blocking software on devices that will interface with the
     server. The ad blocking
     software occasionally misinterprets server resources as ads.
   - Ensure that Google Chrome is installed and is the preferred browser.
   - Important note: Firefox browser is not supported!
   - If it has been more than a few days since the software was released and
     you have internet access, perform a data download before creating the
     event to ensure team info is up to date. "Event Admin" dropdown ->
     Manage Server -> Data Download

