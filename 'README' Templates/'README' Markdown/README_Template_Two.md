Table of contents

TOCs are optional but appreciated for lengthy README files.

CONTENTS OF THIS FILE
---------------------

 * Introduction
 * Requirements
 * Recommended modules
 * Installation
 * Configuration
 * Troubleshooting
 * FAQ
 * Maintainers

Introduction

The introduction (required) shall consist of a brief paragraph or two that summarizes the purpose and function of this project. This introduction may be the same as the first paragraph on the project page.

The introduction should include a link to the project page and issue queue. If the project is a sandbox, these links should go to the sandbox until promotion.

INTRODUCTION
------------

The Administration Menu module displays the entire administrative menu tree
(and most local tasks) in a drop-down menu, providing administrators one- or
two-click access to most pages.  Other modules may also add menu links to the
menu using hook_admin_menu_output_alter().

 * For a full description of the module, visit the project page:
   https://www.drupal.org/project/admin_menu

 * To submit bug reports and feature suggestions, or track changes:
   https://www.drupal.org/project/issues/admin_menu

Requirements

The requirements section (required) shall make it clear whether this project requires anything outside of Drupal core to work (modules, libraries, etc). List all requirements here, including those that follow indirectly from another module, etc. The idea is to inform the users about what is required, so that everything they need can be procured and included in advance of attempting to install the module. If there are no requirements, write "No special requirements".

REQUIREMENTS
------------

This module requires the following modules:

 * [Views](https://www.drupal.org/project/views)
 * [Panels](https://www.drupal.org/project/panels)

REQUIREMENTS
------------

This module requires no modules outside of Drupal core.

Recommended modules

This optional section lists modules that are not required, but that may enhance the usefulness or user experience of your project. Make sure to describe the benefits of enabling these modules.

RECOMMENDED MODULES
-------------------

 * [Markdown filter](https://www.drupal.org/project/markdown):
   When enabled, display of the project's README.md help will be rendered
   with markdown.

Installation

The installation section (required*) shall make it clear how to install the module. However, if the steps to install the module follow the standard instructions for Drupal 8, Drupal 7, Drupal 6/5, or a theme, don't reinvent the wheel — simply provide a link and explain in detail any steps that may diverge from these steps. Take special note of Drush integrations. In a case where many Drush commands are added, consider adding a section for Drush.

Consider replacing this section with a standalone INSTALL.txt file if your installation instructions are especially complex.

* - required unless a separate INSTALL.txt is provided.
Drupal 7

INSTALLATION
------------
 
 * Install as you would normally install a contributed Drupal module. Visit
   https://www.drupal.org/node/895232/ for further information.

 * You may want to disable Toolbar module, since its output clashes with
   Administration Menu.

Drupal 8

INSTALLATION
------------

 * Install as you would normally install a contributed Drupal module. Visit
   https://www.drupal.org/node/1897420 for further information.

Configuration

The configuration section (required) is necessary even when little configuration is required. Use this section to list special notes about the configuration of this module – including but not limited to permissions. This section is particularly important if the module requires additional configuration outside of the Drupal UI.

If the module has little or no configuration, you should use this space to explain how enabling/disabling the module will affect the site.

CONFIGURATION
-------------
 
 * Configure the user permissions in Administration » People » Permissions:

   - Use the administration pages and help (System module)

     The top-level administration categories require this permission to be
     accessible. The administration menu will be empty unless this permission
     is granted.

   - Access administration menu

     Users with this permission will see the administration menu at the top of
     each page.

   - Display Drupal links

     Users with this permission will receive links to drupal.org issue queues
     for all enabled contributed modules. The issue queue links appear under
     the administration menu icon.

 * Customize the menu settings in Administration » Configuration and modules »
   Administration » Administration menu.

 * To prevent administrative menu items from appearing twice, you may hide the
   "Management" menu block.

or

CONFIGURATION
-------------

The module has no menu or modifiable settings. There is no configuration. When
enabled, the module will prevent the links from appearing. To get the links
back, disable the module and clear caches.

Troubleshooting & FAQ

These sections are optional. If present, they should address questions that are asked frequently in the issue queue (this will save you time in the future). Outline common problems that people encounter along with solutions (links are okay if the steps are long, but it is often helpful to provide a summary since links sometimes go stale).

TROUBLESHOOTING
---------------

 * If the menu does not display, check the following:

   - Are the "Access administration menu" and "Use the administration pages
     and help" permissions enabled for the appropriate roles?

   - Does html.tpl.php of your theme output the $page_bottom variable?

FAQ
---

Q: I enabled "Aggregate and compress CSS files", but admin_menu.css is still
   there. Is this normal?

A: Yes, this is the intended behavior. the administration menu module only loads
   its stylesheet as needed (i.e., on page requests by logged-on, administrative
   users).

Maintainers

This section is optional and should replace any pre-existing standalone MAINTAINERS.txt file.

MAINTAINERS
-----------

Current maintainers:
 * Daniel F. Kudwien (sun) - https://www.drupal.org/user/54136
 * Peter Wolanin (pwolanin) - https://www.drupal.org/user/49851
 * Stefan M. Kudwien (smk-ka) - https://www.drupal.org/user/48898
 * Dave Reid (Dave Reid) - https://www.drupal.org/user/53892

This project has been sponsored by:
 * UNLEASHED MIND
   Specialized in consulting and planning of Drupal powered sites, UNLEASHED
   MIND offers installation, development, theming, customization, and hosting
   to get you started. Visit https://www.unleashedmind.com for more information.

Advanced help 

Advanced help will display the README file on the screen if it is enabled.
All about Markdown

During the Drupal project's lifetime, there has never been a clear consensus about what a README-file should look like, and many different styles exist as a result (see links below). However, we prefer new projects to use the format described on this page, or a format recognized by the Markdown filter module. If you use Markdown, your file should be named README.md (and use valid Markdown syntax), otherwise it should be named README.txt.
Quick formatting tips

Here is a summary of the preferred format for README.txt:

    Headings in all caps.
    Headings underlined with ===/--- to the length of the heading, followed by a blank line.
    Two lines prior to headings (except the first one).
    Bullets denoted by asterisks (*) with hanging indents.
    Numbered lists indented 4 spaces.
    Bulleted lists indented 1 space.
    Text manually word-wrapped within around 80 cols.
