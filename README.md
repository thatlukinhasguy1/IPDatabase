# IP Database
An SQLite database of IP address blocks used to detect various types of IP addresses.

**Free for non-commercial projects and products. Get in touch if you require it for commercial projects and products.**

# How to use?
The database is stored in an SQLite database file. You can query like this: `SELECT * FROM IPv4 WHERE Start <= ? AND End >= ?;` where ? is the IP address as an integer.

Example Response:
```
{
  "Start": 16843008,
  "End": 16843008,
  "ASN": "AS13335",
  "Country": "US",
  "City": "Los Angeles",
  "Region": "California",
  "Longitude": "-118.243568",
  "Latitude": "34.05286",
  "Postal": "90001",
  "ISP": "CLOUDFLARENET",
  "Types": "2, 5"
}
```

# Address types:
1. Residential
2. Business
3. Hosting
4. VPN
5. DDoS Mitigation
6. Tor Relay
7. Cloud Gaming
8. Mobile Carrier

# How to add or update ASN's/Blocks/Addresses?
You can request these to be added or updated by opening an issue and providing the following:
```
ASN/Block/Address
[Types]
ASN/Block/Address Holder
Country
City
Region
Longitude
Latitude
Postal
```
*Only the ASN/Block/Address and the outdated fields are required if you are requesting data to be updated.*

# Projects using this:
* [YAAntiVPN](https://github.com/Ameliaaaaaaa/YAAntiVPN)

Get yours listed here by opening a pull request!
