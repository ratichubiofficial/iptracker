import requests

def track_ip(ip_address):
    url = f"http://ipinfo.io/{ip_address}/json"
    response = requests.get(url)
    data = response.json()

    if 'error' in data:
        print(f"Error: {data['error']}")
    else:
        print(f"IP Address: {data['ip']}")
        print(f"Hostname: {data['hostname']}")
        print(f"City: {data['city']}")
        print(f"Region: {data['region']}")
        print(f"Country: {data['country']}")
        print(f"Location: {data['loc']}")
        print(f"Organization: {data.get('org', 'N/A')}")
        print(f"ISP: {data.get('isp', 'N/A')}")

if __name__ == "__main__":
    ip_address = input("Enter an IP address to track: ")
    track_ip(ip_address)
