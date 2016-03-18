# Icinga Web 2 Module "network_services"

Icinga Web 2 Module "network_services" is a bulk import tool for hosts and hosts' systemd services of a local network. 

## Dependencies
- Icinga 2
- Icinga Web 2
- GNU/Linux
- systemd
- OpenSSH
- Nmap

## Installation

- sudo mv icinga_network-services.timer /usr/lib/systemd/system/
- sudo mv icinga_network-services.service /usr/lib/systemd/system/
- sudo mkdir /etc/icingaweb2/modules/network-services/
- sudo cp -R * /etc/icingaweb2/modules/network-services/
- sudo chmod +x /etc/icingaweb2/modules/network-services/scanner
- sudo bash /etc/icingaweb2/modules/network-services/scanner
- sudo systemctl start icinga_network-services.timer
- sudo systemctl start icinga_network-services.service
- sudo systemctl enable icinga_network-services.timer
- sudo systemctl enable icinga_network-services.service

## License

Copyright (C) 2016 Jürgen Hecht

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version. This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

Licensed under the GNU GPLv3: https://www.gnu.org/licenses/gpl-3.0.html

