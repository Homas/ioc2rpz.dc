# ioc2rpz.dc
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)  

## Short summary
ioc2rpz™: The DNS Security Solution - ioc2rpz™ is a powerful DNS server that transforms threat indicators into actionable Response Policy Zone (RPZ) feeds. It automates the update process, ensuring your network is protected against the latest threats, including malicious domains and IP addresses. By converting IOC feeds into RPZs, ioc2rpz™ acts as a crucial link between threat intelligence and DNS security, compatible with RPZ-supporting DNS servers like ISC Bind or PowerDNS.

## Overview
Easily run ioc2rpz™, ioc2rpz.gui on Docker with Docker Compose. ioc2rpz™ is shipped with preconfigured RPZ feeds based on open source threat intelligence (OSINT).

## Prerequisites
- ioc2rpz™ and ioc2rpz.gui use tthe following ports: 53/udp, 53/tcp, 853/tcp, 80/tcp, 443/tcp, 8443/tcp. Ensure that no any other services are using these ports.
- recent releases Docker and Docker Compose

## Configuration
Clone the repository to a directory where you want to deploy the service. During the first service start ioc2rpz.gui startup script will create the following directories with the following content:
- ioc2rpz/cfg - ioc2rpz™ configuration file, a sample whitelist and a temporary ssl certificate and a key;
- ioc2rpz/db - configuration database;
- ioc2rpz/ssl - certificates for ioc2rpz.gui.

## Start ioc2rpz™ service
To start the service execute the following command:
```
sudo docker-compose up -d
```

Refer the docker compose documentation to learn how to restart, stop the service and cleanup.

# Do you want to support to the project?
You can suppor the project via [GitHub Sponsor](https://github.com/sponsors/Homas) (recurring payments) or make one time donation via [PayPal](https://paypal.me/ioc2rpz).

# Contact us
You can contact us by email: feedback(at)ioc2rpz[.]net or in [Telegram](https://t.me/ioc2rpz).

# License
Copyright 2017 - 2024 Vadim Pavlov ioc2rpz[at]gmail[.]com

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License.
You may obtain a copy of the License at  
  
    http://www.apache.org/licenses/LICENSE-2.0  
  
Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
