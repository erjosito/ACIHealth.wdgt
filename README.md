ACI Health Mac OS X Desktop Widget

Prerequisites:
- You need to have Python in your system
- You need to have the requests Python module installed
- HTTPS does not always work (depends on APIC certificate and SSL negotiation)

Installation:
- Clone the git repository to your machine:
   git clone https://github.com/erjosito/ACIHealth.wdgt
- Double click on the downloaded package to install the widget

v0.1
- Initial concept
- Preferences (URL, user, password)
- 3 panels, based on HTML tables

v0.2
- Tables reformatted with CSS
- Including different colors depending on health level / fault severity
- Opens up the APIC GUI on default browser when clicking the widget

v0.3
- Bug in Python scripts for loop
- Set title after options pop up
- verify=False in Python requests. SSL still not working for me,
  there seems to be some dependencies with the requests version

v0.4
- Use the system python (output of a /usr/bin/which python)
- Detect whether APIC reachable
- Detect whether Python libraries in the system