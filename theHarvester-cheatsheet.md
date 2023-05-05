**Introduction**

TheHarvester is a popular open-source tool used by penetration testers, security researchers, and hackers to gather valuable information during the reconnaissance phase. The tool automates the process of data collection by searching for emails, subdomains, hostnames, and employee names associated with a target domain. TheHarvester can use various data sources such as search engines, social networks, and public databases to collect information.

**Usage**

Breakdown of the parameters and options:

```
theharvester -d <domain> -l <limit> -b <source>
```

* `-d`: The target domain to search for. This can be a domain name or an IP address.
* `-l`: The limit of results to display. The default value is 500.
* `-b`: The data source to use. This can be one of the supported data sources such as Google, Bing, LinkedIn, etc.

TheHarvester supports several data sources, each with its own syntax and options. Here's a summary of the most popular data sources:

**Google**

The Google data source searches for emails, subdomains, and hosts using the Google search engine. Here's how you can use the Google data source:

```
theharvester -d <domain> -b google -l <limit>
```

* `-d`: The target domain to search for.
* `-b`: The data source to use, which is Google in this case.
* `-l`: The limit of results to display. The default value is 500.

The Google data source also supports several options that allow you to customize your search. Here are some of the most useful options:

* `-s`: The start page of the search. You can use this option to skip the first few pages of results. The default value is 0.
* `-t`: The search type, which can be either "web" or "dns". The default value is "web".
* `-c`: The country to search from. This option is useful if you want to limit your search to a specific country. The default value is "com".

**Bing**

The Bing data source searches for emails, subdomains, and hosts using the Bing search engine. Here's how you can use the Bing data source:

```
theharvester -d <domain> -b bing -l <limit>
```

* `-d`: The target domain to search for.
* `-b`: The data source to use, which is Bing in this case.
* `-l`: The limit of results to display. The default value is 500.

The Bing data source also supports several options that allow you to customize your search. Here are some of the most useful options:

* `-s`: The start page of the search. You can use this option to skip the first few pages of results. The default value is 0.
* `-t`: The search type, which can be either "web" or "dns". The default value is "web".
* `-c`: The country to search from. This option is useful if you want to limit your search to a specific country. The default value is "com".

**LinkedIn**

The LinkedIn data source searches for employee names using the LinkedIn social network.

```
theharvester -d <domain> -b linkedin -l <limit>
```

* `-d`: The target domain to search for.
* `-b`: The data source to use, which is LinkedIn in this case.
* `-l`: The limit of results to display. The default value is 500.

The LinkedIn data source also supports several options that allow you to customize your search:

* `-u`: The LinkedIn username to use for authentication. This option is required if you want to search for non-public profiles.
* `-p`: The LinkedIn password to use for authentication. This option is required if you want to search for non-public profiles.
* `-c`: The country to search from. This option is useful if you want to limit your search to a specific country. The default value is "us".

**Email/Phone Number/Name**
If you want to look up a specific name, phone number, email address, or other piece of information, you can use TheHarvester to search for that information across multiple search engines and data sources. Here are some examples of how you can use TheHarvester to search for specific information:

To search for a specific email address:

```
theharvester -d <domain> -b google -s <search term>
```

* `-d`: The target domain to search for.
* `-b`: The data source to use, which is Google in this case.
* `-s`: The search term, which is the email address you want to search for.

To search for a specific phone number:

```
theharvester -d <domain> -b google -s <search term>
```

* `-d`: The target domain to search for.
* `-b`: The data source to use, which is Google in this case.
* `-s`: The search term, which is the phone number you want to search for.

To search for a specific name:

```
theharvester -d <domain> -b all -f <first name> -l <last name>
```




**DNSDumpster**

The DNSDumpster data source searches for subdomains using the DNSDumpster database. Here's how you can use the DNSDumpster data source:

```
theharvester -d <domain> -b dnsdumpster -l <limit>
```

* `-d`: The target domain to search for.
* `-b`: The data source to use, which is DNSDumpster in this case.
* `-l`: The limit of results to display. The default value is 500.

The DNSDumpster data source also supports several options that allow you to customize your search. Here are some of the most useful options:

* `-c`: The country to search from. This option is useful if you want to limit your search to a specific country. The default value is "us".
