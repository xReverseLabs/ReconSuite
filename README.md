
# ReconSuite

![ReconSuite Logo](https://raw.githubusercontent.com/xReverseLabs/ReconSuite/main/screenshot/menu.png)

**ReconSuite** is a powerful and efficient multi-tool for domain reconnaissance and network scanning. It combines several essential tools into one suite, providing fast and comprehensive results. Built with Go, ReconSuite leverages high-performance APIs from [xReverseLabs](https://xreverselabs.my.id) to deliver top-notch results for Reverse IP lookup, Subdomain scanning, Domain grabbing, and Proxy grabbing.

## Features

- **Reverse IP Lookup**: Identify domains hosted on a specific IP address.
- **Subdomain Scanner**: Discover subdomains associated with a domain.
- **Domain Grabber by Date**: Retrieve domains registered within a specific date range.
- **Proxy Grabber**: Fetch lists of proxies (HTTP, HTTPS, SOCKS4, SOCKS5) from reliable sources.

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/xReverseLabs/ReconSuite.git
   cd ReconSuite
   ```

2. **Configure API Key:**

   add your API key from [xReverseLabs Clientarea](https://xreverselabs.my.id/clientarea/) to `config.json`

   ```json
   {
       "apiKey": "your_api_key_here",
       "threads": 50
   }
   ```

3. **Run Program:**

   Ensure you have Go installed on your system. Then, install the required Go modules:

   ```bash
   ReconSuite.exe
   ```
  

## Usage

ReconSuite offers a simple command-line interface (CLI) to access its various features. Below is a guide on how to use each tool.

### 1. Reverse IP Lookup

![ReconSuite Logo](https://raw.githubusercontent.com/xReverseLabs/ReconSuite/main/screenshot/reverseip.png)

```bash
ReconSuite.exe
```
- Select `1. Reverse IP Lookup`.
- Enter the path to your IP list file.
- The tool will output the domains found on each IP to `ReverseIP_Result.txt`.

### 2. Subdomain Scanner
![ReconSuite Logo](https://raw.githubusercontent.com/xReverseLabs/ReconSuite/main/screenshot/subdoscan.png)
```bash
ReconSuite.exe
```
- Select `2. Subdomain Scanner`.
- Enter the path to your domain list file.
- The tool will output the subdomains found for each domain to `Subdomain_Results.txt`.

### 3. Domain Grabber by Date
![ReconSuite Logo](https://raw.githubusercontent.com/xReverseLabs/ReconSuite/main/screenshot/domainbydate.png)

```bash
ReconSuite.exe
```
- Select `3. Domain Grabber by Date`.
- Enter the start date (YYYY-MM-DD).
- Enter the end date (YYYY-MM-DD).
- The tool will retrieve domains registered between the specified dates and output them to `Grabbed.txt`.

### 4. Proxy Grabber
![ReconSuite Logo](https://raw.githubusercontent.com/xReverseLabs/ReconSuite/main/screenshot/proxy.png)

```bash
ReconSuite.exe
```
- Select `4. Proxy Grabber`.
- Choose the type of proxies you want to grab (HTTP, HTTPS, SOCKS4, SOCKS5, ALL).
- The tool will output the proxies to `Proxies.txt`.

## Contributing

We welcome contributions! Please open an issue or submit a pull request with your improvements. Follow the standard Go formatting and write clear commit messages.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **[xReverseLabs](https://xreverselabs.my.id)** for providing the high-quality APIs that power this tool.
- The Go community for creating such a powerful and efficient programming language.
