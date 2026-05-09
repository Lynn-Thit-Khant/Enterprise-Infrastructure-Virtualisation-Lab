# Linux Web Server Setup

## Purpose

Linux web servers were deployed to provide regional web services.

## Basic Apache Setup

```bash
sudo apt update
sudo apt install apache2 -y
sudo systemctl enable --now apache2
sudo systemctl status apache2
```

## Validation

Test Apache locally or from another VM:

```bash
curl http://<web-server-ip>
```

Example web server IPs:

| Server | IP Address |
|---|---|
| Web-SG | 172.16.110.86 |
| Web-TH | 172.16.110.64 |
| Web-JP | 172.16.110.37 |
| Web-TW | 172.16.110.62 |

## Notes

Each Linux web server was kept lightweight to focus on infrastructure design, connectivity, storage, and recovery validation.
