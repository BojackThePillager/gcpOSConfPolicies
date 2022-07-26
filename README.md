# gcpOSConfPolicies
Google Cloud Platform Compute OS Configuration Policies

Google Cloud Platform has a handy capability to write yaml based files that allow inspection and/or enforcement of system states. 

I decided that this would be a handy way for a red team to remotely do things like have the target cloud compute instance do all the things red teams like to do like: -download files, -run executables, -install software, etc. 

What's great is if Blue team or an admin discovers the activity and deletes the file or kills the process then GCP OS Configuration Management will just re-download the file and make sure it is running. 

The only downside is that you need to tailor the GCP OS configuration policy script files specifically to the operating system version you are targeting which results in creating more OS policy files. As I experiement and create more OS policy files I will add them into this repo. 
