# richfaces-impl-patched
The original richfaces-impl.3.3.4.Final, but with all the whitelisted classes removed from resource-serialization.properties

Several vulnerabilities (such as CVE-2018-12533 and CVE-2018-14667) are based on the fact that under certain circumstances RichFaces deserializes classes based on a whitelist, which is defined in a file called resource-serialization.properties .

If you don't need the functionality where this is involved, then you can defend against these attacks by emptying the whitelist --> which is exactly what is done here.
