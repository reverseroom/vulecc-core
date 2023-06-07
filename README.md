## VULECC
VULECC is the pioneer in Next-Generation Web Application Vulnerability Scanning technology, enabling businesses to proactively probe their web assets to identify and combat the most intricate vulnerabilities.

VULECC is at the forefront of Next-Generation Web Vulnerability Scanning technology. Designed to facilitate proactive security, it enables organizations to rigorously scrutinize their web technologies and identify even the most sophisticated vulnerabilities. VULECC's advanced algorithms simulate real-world attack scenarios, providing a comprehensive insight into potential security loopholes that may be exploited by cybercriminals.

<p align="center">
<img src="https://i.imgur.com/jzGqt6G.png" width="300" />
</p>

VULECC navigates the complex landscape of web technologies - from legacy HTML websites to cutting-edge JavaScript applications, content management systems, and APIs. It's adept at detecting a wide range of web-specific vulnerabilities, including SQL Injection, Cross-Site Scripting (XSS), Cross-Site Request Forgery (CSRF), and various other OWASP Top 10 security risks. This makes VULECC an all-encompassing security solution for web applications.

The scanner provides comprehensive reports, detailing the detected vulnerabilities and providing remediation guidance, making it an invaluable tool for both security experts and IT professionals. Furthermore, it prioritizes detected vulnerabilities based on their potential impact, allowing teams to effectively allocate resources and tackle the most significant threats first.

What sets VULECC apart is its ability to adapt to the constantly evolving landscape of cyber threats. By utilizing advanced machine learning algorithms and AI technology, VULECC ensures its vulnerability scanning capabilities remain at the cutting edge, always ready to respond to new vulnerabilities and exploits as they emerge.
Whether you're a small business or a multinational corporation, VULECC offers a proactive, end-to-end solution to safeguard your digital assets, helping you maintain a resilient and secure IT environment. It is an indispensable tool in a world where cyber threats are increasingly sophisticated and prevalent. VULECC offers the peace of mind that comes from knowing your digital assets are safe, secure, and well-managed.

## Download Vulecc CLI

You need to download Vulecc CLI package to run Vulecc:

```shell
curl -fsSL https://dashboard.vulecc.com/download -o vulecc.tar.gz
tar -xvzf vulecc.tar.gz
```

## Start a Vulecc launcher

```shell
Usage: vulecc-cli --target <TARGET> --bundle <BUNDLE> --scripts <SCRIPTS> --group <GROUP> --client-id <CLIENT_ID> --parallel <PARALLEL>

Options:
  -t, --target <TARGET>        Target URL
  -b, --bundle <BUNDLE>        File path for the bundle package
  -s, --scripts <SCRIPTS>      List of scripts to run (comma-separated, file)
  -g, --group <GROUP>          Script group name which contains multiple scripts
  -c, --client-id <CLIENT_ID>  Client ID value
  -p, --parallel <PARALLEL>    Parallel thread count for DynaScan
  -h, --help                   Print help
```

To run Vulecc, you should pass your client ID to the Vulecc CLI. To do this, log in to your account and copy the client ID from the dashboard.

## Command-line arguments

| Argument      | Meaning                                                                                                    |
| ------------- | -----------------------------------------------------------------------------------------------------------|
| target        | The target URL of your website for the vulnerability scan.                                                 |
| bundle        | The file path for the bundle package, which defaults to 'vulecc.bin'.                                      |
| scripts       | List of individual script names to run (e.g: `./bundler/Community/sql_injection.lua`)                      |
| group         | Script group name which contains multiple script name (e.g: datastores, accesscontrol etc.)                |
| client-id     | Validation of your license is accomplished using the client ID value.                                      |
| parallel      | The parallel value is used to enhance the speed of Dynascan by increasing the count of parallel instances. |
