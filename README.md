# gcpOSConfPolicies
Google Cloud Platform GCE OS Configuration Policies

Google Cloud Platform has a handy capability to write yaml based files that allow GCE to perform inspection and/or enforcement of system states on compute instances. 

I decided that this would be a handy way for a red team to remotely do things on the target cloud compute instance like -download files, -run executables, -install software, etc. AND make sure it stays that's way...

Note: GCP OS Configuration Manager runs it on the hosts as root or run sudo without password to make sure.

What's great is if Blue team or an admin discovers the activity and deletes the file or kills the process then GCP OS Configuration Management will just re-download the file and make sure it keeps running. 

The only downside is that you need to tailor the GCP OS configuration policy script files specifically to the operating system version you are targeting which results in creating more OS policy files. As I experiement and create more OS policy files I will add them into this repo.
