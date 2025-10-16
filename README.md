# SOCKS4 Proxy List 🔒

A comprehensive collection of **500+ working SOCKS4 proxy servers** in plain text format for easy integration into your applications and tools.

## 📊 Statistics

- **Total Proxies**: 500
- **Format**: Plain text (IP:PORT)
- **Protocol**: SOCKS4
- **Sources**: 22 different proxy providers
- **Last Updated**: October 16, 2025

## 📁 Files

- `socks4-proxies.txt` - Main proxy list file (500+ SOCKS4 proxies)
- `README.md` - This documentation

## 🚀 Usage

### Direct Download
```bash
curl -O https://raw.githubusercontent.com/Blacky1999/socks4-proxy-list/main/socks4-proxies.txt
```

### Using wget
```bash
wget https://raw.githubusercontent.com/Blacky1999/socks4-proxy-list/main/socks4-proxies.txt
```

### In Python
```python
import requests

response = requests.get('https://raw.githubusercontent.com/Blacky1999/socks4-proxy-list/main/socks4-proxies.txt')
proxy_list = response.text.strip().split('\n')

for proxy in proxy_list:
    print(f"SOCKS4 Proxy: {proxy}")
```

### In Node.js
```javascript
const fetch = require('node-fetch');

fetch('https://raw.githubusercontent.com/Blacky1999/socks4-proxy-list/main/socks4-proxies.txt')
  .then(response => response.text())
  .then(data => {
    const proxies = data.trim().split('\n');
    proxies.forEach(proxy => {
      console.log(`SOCKS4 Proxy: ${proxy}`);
    });
  });
```

## 🔧 Integration Examples

### ProxyChains Configuration
Add to your `/etc/proxychains.conf`:
```
[ProxyList]
socks4 181.48.160.114 9090
socks4 8.213.129.20 3132
socks4 184.178.172.28 15294
# ... add more proxies as needed
```

### Curl with SOCKS4 Proxy
```bash
curl --socks4 181.48.160.114:9090 https://httpbin.org/ip
```

### Requests with SOCKS Proxy (Python)
```python
import requests

proxies = {
    'http': 'socks4://181.48.160.114:9090',
    'https': 'socks4://181.48.160.114:9090',
}

response = requests.get('https://httpbin.org/ip', proxies=proxies)
print(response.json())
```

## 📊 Proxy Sources

This list aggregates proxies from multiple reliable sources:
- ProxyScrape
- TheSpeedX/PROXY-List
- Free-Proxy-World
- GeoNode Proxy List
- Advanced.name
- ProxyTools.com
- ProxyBros.com
- Hide.me
- Spys.one
- And many more...

## ⚠️ Important Notes

- **Testing Required**: Always test proxies before use in production
- **No Uptime Guarantee**: Free proxies may become unavailable without notice
- **Educational Purpose**: Use responsibly and respect terms of service
- **No Authentication**: These are public, anonymous SOCKS4 proxies
- **Security Warning**: Do not send sensitive data through free proxies

## 🔄 Updates

This list will be updated regularly with fresh working proxies. Check back frequently for the latest additions.

## 📜 Format

Each line contains one proxy in the format:
```
IP_ADDRESS:PORT
```

Example:
```
181.48.160.114:9090
8.213.129.20:3132
184.178.172.28:15294
```

## 🤝 Contributing

Feel free to contribute by:
- Reporting dead proxies
- Suggesting new proxy sources
- Improving documentation
- Creating issues for bugs or improvements

## 📧 Contact

- GitHub: [@Blacky1999](https://github.com/Blacky1999)

## ⭐ Support

If this proxy list helps you, please consider:
- Starring this repository
- Sharing it with others
- Contributing improvements

---

**Disclaimer**: These proxies are collected from public sources. Use at your own risk and comply with all applicable laws and terms of service.