#  Bilal Gökçen Ay | Senior Cybersecurity Engineer & Game Developer

> _"The best way to predict the future is to create it."_  
> — *Bilal Gökçen Ay*

---

##  Profil Tanımı: `class BilalProfile`

```python
from abc import ABC, abstractmethod
from typing import List, Dict, Optional, Tuple
from dataclasses import dataclass
import datetime

@dataclass
class SystemInfo:
    cpu: str = "Intel i5-14400F"
    gpu: str = "RTX 4060"
    os: str = "Kali Linux 2023.3"
    kernel: str = "Linux 6.5.0-kali1-amd64"

class CyberSecProfile(ABC):
    def __init__(self):
        self.name = "Bilal Gökçen Ay"
        self.role = "Senior Cybersecurity Engineer & Game Developer"
        self.vision = "The best way to predict the future is to create it."
        self.concept = "System Terminal / CyberSec Dashboard"
        self.system_info = SystemInfo()
        self.technologies = {
            "Cybersecurity": ["Python", "Flask", "sqlparse", "Kali Linux", "NTP", "Wireshark"],
            "Game Development": ["Unreal Engine 5.4.4", "C#", "Blender 3D"],
            "Tools": ["Git", "VSCode", "Linux CLI", "Docker"]
        }
        
    @abstractmethod
    def get_bio(self) -> str:
        pass
    
    @abstractmethod
    def get_roadmap(self) -> Dict[str, List[str]]:
        pass

class BilalProfile(CyberSecProfile):
    def __init__(self):
        super().__init__()
        self.commit_count = 120
        self.languages = ["Python", "C#", "Shell Scripting", "SQL"]
        self.projects = 8
        
    def get_bio(self) -> str:
        return f"""
root@bilal:~# whoami
{self.name}

root@bilal:~# role
{self.role}

root@bilal:~# vision
{self.vision}

root@bilal:~# system_info
{self.system_info.cpu}
{self.system_info.gpu}
{self.system_info.os}
{self.system_info.kernel}

root@bilal:~# uptime
 12:45:36 up 2 days,  8:12,  1 user,  load average: 0.03, 0.05, 0.08

root@bilal:~# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda1        46G   21G   23G  48% /

root@bilal:~# ps aux | grep python
bilal     1234  0.0  0.1  12345  6789 ?        S    12:30   0:01 python3 waf_engine.py

root@bilal:~# nmap -sV localhost
Starting Nmap 7.94 ( https://nmap.org ) at 2026-06-15 12:45 CEST
Nmap scan report for localhost (127.0.0.1)
Host is up (0.00012s latency).
Not shown: 998 closed ports
PORT     STATE SERVICE    VERSION
22/tcp   open  ssh        OpenSSH 8.4p1 Debian 5+deb11u1
80/tcp   open  http       Apache httpd 2.4.56

root@bilal:~# git status
On branch main
Your branch is up to date with 'origin/main'

nothing to commit, working tree clean

root@bilal:~# netstat -tuln | grep :80
tcp6  0  0 :::80  :::*  LISTEN  1234/apache2

root@bilal:~# ps aux | grep waf
bilal   1234  0.1  0.2  12345  6789 ?  S    12:30   0:01 python3 waf_engine.py

root@bilal:~# cat /proc/cpuinfo | grep 'model name' | head -1
model name      : Intel(R) Core(TM) i5-14400F CPU @ 2.50GHz

root@bilal:~# lshw -short -C memory
H/W path         Device      Class          Description
=========================================================
/0/100/18.0    memory       Memory controller
/0/100/18.1    memory       Memory controller
/0/100/18.2    memory       Memory controller
/0/100/18.3    memory       Memory controller

root@bilal:~# ls -la /opt/security/
total 24
drwxr-xr-x  5 bilal bilal 4096 Jun 15 12:00 .
drwxr-xr-x  1 root  root  4096 Jun 15 11:30 ..
drwxr-xr-x  5 bilal bilal 4096 Jun 15 12:00 waf_project
drwxr-xr-x  2 bilal bilal 4096 Jun 15 11:45 logs
-rw-r--r--  1 bilal bilal   89 Jun 15 11:35 config.ini
-rw-r--r--  1 bilal bilal  204 Jun 15 11:35 requirements.txt

root@bilal:~# 
        """
    
    def get_roadmap(self) -> Dict[str, List[str]]:
        return {
            "Completed": [
                "TUA Astro Hackathon 2026",
                "Bilim Ümraniye MIT App Inventor",
                "Version Control Systems (VCS)"
            ],
            "Current": [
                "ISMEK Siber Güvenlik ve Sızma Testi kursu (Haziran 2026)",
                "Unreal Engine 5.4.4 Game Development"
            ],
            "Future": [
                "TCMB Stajı (12. Sınıf)",
                "Advanced WAF Development",
                "AI-Powered Anomaly Detection"
            ]
        }

# Instantiate the profile
profile = BilalProfile()

GitHub İstatistikleri
https://github-readme-stats.vercel.app/api?username=bilalgokcen&show_icons=true&theme=dark&hide_border=true&card_width=400
https://github-readme-stats.vercel.app/api/top-langs/?username=bilalgokcen&layout=compact&theme=dark&hide_border=true&card_width=400

 Teknik Yetkinlikler
 https://www.python.org/
 https://docs.microsoft.com/en-us/dotnet/csharp/
 https://www.kali.org/
https://www.unrealengine.com/
https://flask.palletsprojects.com/
https://www.blender.org/
https://www.docker.com/

Siber Güvenlik Uzmanlığı
WAF (Web Application Firewall) Geliştirme
class AdaptiveWAF:
    def __init__(self):
        self.rules = []
        self.anomaly_detector = None
        self.spoofing_protection = True
        
    def detect_anomalies(self, traffic_data):
        # AI-powered anomaly detection logic
        pass
        
    def prevent_spoofing(self, packet_data):
        # Anti-spoofing mechanism
        pass
        
    def adaptive_learning(self, new_patterns):
        # Learning from new attack patterns
        pass

# WAF Engine
waf_engine = AdaptiveWAF()

 TCMB Staj Hedefi
Yıl: 12. Sınıf
Konu: Siber Güvenlik ve Sızma Testi
Hedef: Türkiye Cumhuriyet Merkez Bankası


 Donanım & Sistem Optimizasyonu
 Sistem Bakımı (System Maintenance)

# Bilek ve Parmak Kondisyonu Antrenmanları
root@bilal:~# cat /sys/class/hwmon/hwmon0/temp1_input
35000

# Sistem Performansı
root@bilal:~# iostat -x 1 2
Linux 6.5.0-kali1-amd64 (bilal)   15.06.2026   _x86_64_   (16 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           12.3    0.1     8.7    2.1     0.2    76.6

Device:         rrqm/s   wrqm/s     r/s     w/s   rkB/s   wkB/s avgrq-sz avgqu-sz await svctm %util
nvme0n1           0.00     0.00   25.00   15.00  1000.00  1500.00    80.00     5.00   100.00   10.00  40.00
****

Gaming & High Performance Optimization
RTX 4060 GPU ile 1440p gaming
i5-14400F (P-Core/E-Core) mimarisi
Özel bilek ve parmak kondisyonu antrenmanları

Eğitim & Gelecek Hedefleri
 Tamamlananlar:TUA Astro Hackathon 2026
Bilim Ümraniye MIT App Inventor
Version Control Systems (VCS)
 Gelecek Hedefler:Haziran 2026: ISMEK Siber Güvenlik ve Sızma Testi kursu
12. Sınıf: Türkiye Cumhuriyet Merkez Bankası (TCMB) Stajı
 Profil Bilgileri
Ad: Bilal Gökcen Ay

Rol: Siber Güvenlik Mühendisi Adayı & Oyun Geliştirici

Vizyon: "The best way to predict the future is to create it."
