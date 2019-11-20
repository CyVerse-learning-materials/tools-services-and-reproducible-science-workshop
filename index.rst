|CyVerse logo|

CyVerse Tools, Services, and Reproducibility, Workshop
------------------------------------------------------------

Tools and services workshops cover the major platforms of the CyVerse
cyberinfrastructure (http://www.cyverse.org/) including:


**Day One**

*Introduction to CyVerse*

This workshop covers CyVerse basics from data upload through to analysis and
publication. Ultimately, we will use RNA-Seq as an example analysis. Topics
include:

- **Data Store:** Data storage, sharing, metadata management, and the Data Commons
- **Discovery Environment:** A web-based, graphical interface to hundreds of
  bioinformatics tools
- **Atmosphere:** Custom cloud computing for life science
- **RNA-Seq**: A demonstration of data analysis, we will use the Kallisto/Sleuth
  workflow to analyze RNA-Seq data.

*Workshop Level*

This workshop focuses on beginning users with little to no previous bioinformatics
experience. For the RNA-Seq analysis, some familiarity with R will be helpful

----

**Day Two**

Reproducible Science with CyVerse

This workshop focuses on essentials for reproducible science. The emphasis is
on how to manage software and code to generate research that can be more easily
replicated and that complies with modern publication and funding agency
standards. Topics include:

- **Implementing FAIR**: Understanding and implementing the |FAIR| principles
  and |4OSS| recommendations.
- **Jupyter Notebooks**: Using notebooks for reproducible analysis
- **Docker**: Using, managing, and creating containers for software
  reproducibility
- **Tool Installation on CyVerse**: Deploying applications on CyVerse

*Workshop Level*

This workshop is more suited for intermediate and advanced users interested in
extending and customizing CyVerse capabilities, including installing their own
tools. Familiarity of Linux/command line is highly recommended.


-----

Pre-Workshop Setup
---------------------

**Minimum Setup Instructions Day One**

.. list-table::
    :header-rows: 1

    * - Prerequisite
      - Notes
      - Links
    * - Wi-Fi-enabled laptop (Mac or Linux recommended)
      - You should be able to use CyVerse from any laptop using
        Windows/MacOS/Linux. We **Strongly recommend** having access to a laptop
        running Windows/MacOS. While you will be able to use CyVerse components
        from any laptop, some of the tool installations may work better with
        those operating systems. **For the day two workshop** If you are using
        Windows, you may wish to install |Linux Bash for Windows|.
        We also **strongly recommend** Firefox or Chrome browser; **We do not**
        **recommend Microsoft Edge Browser**. It is helpful if you have
        administrative/install permissions on your laptop. **Note:** If
        specified, some workshops will be held in computer labs in which case a
        laptop is optional.
      - - |Download FireFox|
        - |Download Chrome|
    * - CyVerse Account
      - Please ensure you have a CyVerse account and have **verified** your
        account by completing the verification steps in the email you got when
        you registered. You can **test your account** by logging
        into |CyVerse User Portal|.
      - Register for your CyVerse account at |CyVerse User Portal|.
        Please register using an institutional email address (e.g.
        .edu/.gov/.org etc.).
    * - Atmosphere Access
      - After registering for a CyVerse account, you will need to request access
        to Atmosphere. Instructions for registering for access are `here <https://cyverse-atmosphere-guide.readthedocs-hosted.com/en/latest/>`_
        (See note marked **Important**). **Atmosphere Access may take 24 hours**
        so please do this in advance. **Verify your Atmosphere Access** by
        logging in: |Atmosphere|.
        For justification, you can indicate you are requesting access for a workshop.
      - Request Atmosphere access at the CyVerse user portal |CyVerse User Portal|.
    * - Cyberduck
      - Cyberduck is a third-party tool for uploading/downloading data to CyVerse.
        Currently, this tool is available for Windows/MacOS only. You will need
        to download Cyberduck and the connection profile. We will go through
        configuration and installation at the workshop.
      - |Download Cyberduck|

**Minimum Setup Instructions Day Two**

.. list-table::
    :header-rows: 1

    * - Prerequisite
      - Notes
      - Links
    * - Docker
      - Docker is a technology for running individual software tools in a
        reproducible environment, and on any machine. We request you install
        The **Desktop, Community Edition** of Docker if you are using
        Windows or MacOS. The **Docker CE x86_64** instructions are also
        available for Linux users. If you have installation problems, we
        will also have backup cloud instances available.
      - |Download Docker|
    * - Git
      - Git is a version control software.
        If you are using Linux or MacOS, you most likely already have Git.
        Windows users may need to install Git. You can find instructions
        for Git installation at the link.
      - |Install Git|
    * - Text editor
      - You will need to have a text editor suitable for working with code
        (*Not* Microsoft word, or other word processing software).
      - We recommend installing |Atom|

**Accounts**

.. list-table::
    :header-rows: 1
    * - Prerequisite
      - Notes
      - Links
    * - Github
      - We will make use of Github for managing documentation, and also any
        software/scripts developed (E.g. Docker files).
      - Register for a |GitHub| account
    * - Dockerhub
      - Dockerhub is an online repository for the sharing and management of
        Docker images.
      - Register for a |Dockerhub| account



**Optional Download Extras**

These are some extra downloads that aren't required for the workshop, but which
provide some options for functionalities we will cover.

.. list-table::
    :header-rows: 1

    * - Tool
      - Notes
      - Link
    * - PuTTY (windows only)
      - PuTTY allows SSH connection to a remote machine, and is designed for
        Windows users who do not have a Mac/Linux terminal.
      - `Download PuTTY <https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html>`_
    * - iCommands
      - iCommands are third-party software for command-line connection to the
        CyVerse Data Store.
      - Download and installation instructions available at `CyVerse Learning Center <https://cyverse-data-store-guide.readthedocs-hosted.com/en/latest/step2.html>`__

----

Agenda
--------

 - Prior to the workshop, please take the `Pre-workshop Survey <https://www.surveymonkey.com/r/ToolsServices_pre>`_.

**Day One: CyVerse Tools and Services**

.. list-table::
    :header-rows: 1

    * - Time
      - Topic/Activity
      - Slides
      - Guides
      - Notes/Links
    * - 9:30-10:00
      - Introduction to CyVerse
      - `slides <https://github.com/CyVerse-learning-materials/cyverse_tools_and_services_workshop/raw/master/slides/tsw_intro.pptx>`__
      -
      -
    * - 10:00-10:30
      - Data Management Basics and Data upload with Cyberduck
      - `slides <https://github.com/CyVerse-learning-materials/cyverse_tools_and_services_workshop/raw/master/slides/data_store.pptx>`__
      - `guide <https://cyverse-data-store-guide.readthedocs-hosted.com/en/latest/>`__
      - - `Download Cyberduck`_
        - `Download CyVerse Cyberduck connection profile`_
    * - 10:30-10:45
      - Break
      -
      -
      -
    * - 10:45-11:00
      - Data Sharing within CyVerse
      -
      - `guide <https://cyverse-data-store-guide.readthedocs-hosted.com/en/latest/step4.html>`__
      -
    * - 11:00-12:00
      - CyVerse Discovery Environment walkthrough and exercises
      - `slides <https://github.com/CyVerse-learning-materials/cyverse_tools_and_services_workshop/raw/master/slides/discovery_enviornment.pptx>`__
      - `guide <http://learning.cyverse.org/projects/cyverse-discovery-environment-guide/>`__
      - - `FastQC Exercise <https://cyverse-fastqc-quickstart.readthedocs-hosted.com/en/latest/>`_
        - `Trimmomatic Exercise <https://cyverse-trimmomatic-quickstart.readthedocs-hosted.com/en/latest/>`_
    * - 12:00-01:00
      - Lunch
      -
      -
      -
    * - 01:00-01:45
      - Cloud Computing with CyVerse Atmosphere
      - `slides <https://github.com/CyVerse-learning-materials/cyverse_tools_and_services_workshop/raw/master/slides/atmosphere.pptx>`__
      - `guide <https://cyverse-atmosphere-guide.readthedocs-hosted.com/en/latest/>`__
      -
    * - 01:45-02:15
      - Introduction to New RNA-Seq Methods
      - `Kallisto Tutorial <https://cyverse-kallisto-tutorial.readthedocs-hosted.com/en/latest/>`_
      -
      - - `RNA-Seq Best Practicies <https://wiki.cyverse.org/wiki/download/attachments/36470870/Best_Practices_RNA_Seq_ConesaEtal_2016.pdf?version=1&modificationDate=1499770226000&api=v2>`_
        - `Kallisto Paper <https://www.nature.com/nbt/journal/v34/n5/full/nbt.3519.html>`_
    * - 02:15-02:30
      - Break
      -
      -
      -
    * - 03:00-04:30
      - Guided Sleuth Tutorial / Guided Tuxedo 2.0 Tutorial
      -
      -
      - - `Sleuth Tutorial <https://cyverse-kallisto-tutorial.readthedocs-hosted.com/en/latest/step4.html>`_
    * - 04:30
      - Wrap up/conclusion
      -
      -
      - `Post Survey <https://www.surveymonkey.com/r/ToolsServices_post>`_

-----

**Day Two: Reproducibility with CyVerse:


.. list-table::
    :header-rows: 1

    * - Time
      - Topic/Activity
      - Slides
      - Guides
      - Notes/Links
    * - 9:30-10:00
      - Introduction to Open Science principles
      -
      -
      - - |FAIR|
        - |4OSS|
    * - 10:00-10:30
      - Metadata Management  with CyVerse
      -
      -
      -
    * - 10:30-10:45
      - Break
      -
      -
      -
    * - 10:45-11:30
      - Introduction to Jupyter
      -
      -
      -
    * - 11:30-12:00
      - Building workflows with SnakeMake
      -
      -
      -
    * - 12:00-01:00
      - Lunch
      -
      -
      -
    * - 01:00-02:00
      - Introduction to Docker
      -
      -
      -
    * - 02:00-03:00
      - Managing and customizing Docker containers
      -
      -
      -
    * - 02:15-02:30
      - Break
      -
      -
      -
    * - 03:00-04:30
      - Deploying tools on CyVerse
      -
      -
      -
    * - 04:30
      - Wrap up/conclusion
      -
      -
      - 


-----

Host Prep Instructions
------------------------

These instructions are reminders for those hosting a CyVerse Workshop with us or
on their own.

**Internet and Wi-Fi**

Good Wi-Fi is essential to this internet-based workshop. We would advise checking
with your local IT on the ability to connect 20-40 laptops in the room you are
using. Hopefully, you or others have experience on using the space you have reserved.
In addition, please consider that not every attendee may be local (including your CyVerse
traininer) and so restruction-free/guest public Wi-Fi access should be available.

  .. Important::

     On Guest/public Wi-Fi it is not uncommon for certian ports needed to
     communicate with CyVerse services may be blocked. In our experience, IT
     is usually willing to open these ports (or provide temporary gues
     login) for the duration of the workshop. The following ports are needed
     for the workshop:

     - **iRODS/Data Store:** 1247 and 20000-20399
     - **SSH:** 22
     - **VNC:** 5900-5910
     - **RStudio:** 8787
     - **Jupyter:** 8000

Your CyVerse instructor will test connection prior to the workshop, or work with
you to test connection to services.

**Room Spaces/Computer labs**

Our workshops are one to several days in length. A good space will have:

 - Windows (with shades), ventillation and resonably comfortable chairs
 - Sufficent powerstips or power access for laptop users.
 - One or more large projection screens with bright projectors
 - Accomidation for attendees with mobility/hearing/vision difficulties

 If using a Computer Lab, we recommend having the Prerequisite and Download Extras
 installed if possible.

About CyVerse
-------------

**CyVerse Vision:** Transforming science through data-driven discovery.

**CyVerse Mission:** Design, deploy, and expand a national
cyberinfrastructure for life sciences research and train scientists in
its use. CyVerse provides life scientists with powerful computational
infrastructure to handle huge datasets and complex analyses, thus
enabling data-driven discovery. Our powerful extensible platforms
provide data storage, bioinformatics tools, image analyses, cloud
services, APIs, and more.

While originally created with the name iPlant Collaborative to serve
U.S. plant science communities, CyVerse cyberinfrastructure is germane
to all life sciences disciplines and works equally well on data from
plants, animals, or microbes. By democratizing access to supercomputing
capabilities, we provide a crucial resource to enable scientists to find
solutions for the future. CyVerse is of, by, and for the community, and community-driven needs
shape our mission. We rely on your feedback to provide the
infrastructure you need most to advance your science, development, and
educational agenda.

**CyVerse Homepage:** `http://www.cyverse.org <http://www.cyverse.org>`_

Funding and Citations
---------------------

CyVerse is funded entirely by the National Science Foundation under
Award Numbers DBI-0735191 and DBI-1265383.

Please cite CyVerse appropriately when you make use of our resources,
`CyVerse citation
policy <http://www.cyverse.org/acknowledge-cite-cyverse>`__

.. |CyVerse logo| image:: ./img/cyverse_rgb.png
	:width: 500
	:height: 100

.. |platform_stack| image:: ./img/cyverse_platform_stack.png
  :width: 750
  :height: 700
