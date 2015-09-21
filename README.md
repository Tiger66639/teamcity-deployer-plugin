###TeamCity plugin to upload artifacts to external locations
----------------------------
[![Build Status](https://travis-ci.org/Tiger66639/teamcity-deployer-plugin.svg?branch=build-12)](https://travis-ci.org/Tiger66639/teamcity-deployer-plugin)
This plugin adds basic deployment functions
to TeamCity continuous integration server
http://www.jetbrains.com/teamcity/

####Installation

Copy zip archive to %TeamCity_data_dir%/plugins
and restart the server. Agents will be upgraded automatically

####Usage

In build configuration settings, new runners will be available for build steps.
New runners include:
 * SMB Deployer   - upload artifacts via SMB (Windows shares)
 * FTP Deployer   - upload artifacts via FTP
 * SSH Deployer   - upload artifacts via SSH (using SCP or SFTP protocols)
 * SSH Exec       - execute arbitrary commands using SSH
 * Cargo Deployer - deploy WAR application archives to different servlet containers (based on Cargo library: http://cargo.codehaus.org)

 When configuring artifacts for upload, same patterns can be used as in "Artifacts Path" section of "General Settings"
 page. Including packaging artifacts to zip/tgz archives

####License

Apache, version 2.0
http://www.apache.org/licenses/LICENSE-2.0
