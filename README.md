# SOC Automation: Wazuh + Shuffle + TheHive

## Overview
This project creates an automated Security Operations Center (SOC) pipeline for real-time file threat detection and incident response. It integrates Wazuh for threat detection, Shuffle for workflow automation, and TheHive for incident management, with Elasticsearch and Cassandra for log and data management.

## Features
Wazuh: Monitors file downloads and detects threats in real-time.
Shuffle: Automates alert forwarding from Wazuh to TheHive.
TheHive: Centralizes security alerts for efficient incident response.
Future Plans: Integrate Cortex for automated malware analysis and MISP for enhanced threat intelligence.

## Architecture

Ubuntu VM 01: Runs Wazuh Agent to monitor file downloads.

Ubuntu VM 02: Hosts Wazuh Manager and Shuffle for alert processing and automation.

Ubuntu VM 03: Runs TheHive for incident management, supported by Elasticsearch and Cassandra.


## How It Works
Wazuh detects file creation in the monitored directory.
Alerts are sent to Shuffle, which forwards them to TheHive.
TheHive organizes alerts into cases for analysis and response.

## Setup
For detailed installation and configuration steps, refer to the full article: SOC Automation: Wazuh + Shuffle + TheHive.

## Future Enhancements
Add Cortex for automated malware analysis.
Integrate MISP for improved threat intelligence sharing.
integrate virustotal and etc.
