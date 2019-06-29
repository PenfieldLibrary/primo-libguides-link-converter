# How to setup an SRU Server
## Description
This is basic instructions to setup your library SRU server.
## Setup
1. On the Integration Profile List page (<font color="#2C4D82">Configuration Menu > General > External Systems > Integration Profiles</font>), select <b>Add Integration Profile</b>. Page 1 of the External System wizard opens.

2. Enter a unique code for the new integration type.

3. Enter a unique name for the new integration type.

4. Select <b>SRU</b> Server for <b>Integration Type</b>.
```
The Default check box is not functional for this integration type.
```
5. Select <b>Next</b>.

6. Configure the SRU integration profile using the parameter explanations in the table below.

![sample SRU profile](https://github.com/PenfieldLibrary/primo-libguides-link-converter/raw/master/.docs/sample-SRU-profile.png)

## Test your SRU Server URL
```
SRU Server URL
https://<Alma domain>/view/sru/<institution code>

Example SRU Server:
For SUNY Oswego Penfield library
https://suny-osw.primo.exlibrisgroup.com/discovery/search?sortby=rank&vid=01SUNY_OSW:01SUNY_OSW&lang=en

<Alma domain> is https://suny-osw.primo.exlibrisgroup.com

<institution code> is 01SUNY_OSW:01SUNY_OSW

SRU Server
https://suny-osw.primo.exlibrisgroup.com/view/sru/01SUNY_OSW

Server response
<searchRetrieveResponse xmlns="http://www.loc.gov/zing/srw/" xmlns:diag="http://www.loc.gov/zing/srw/diagnostic/">
  <version>1.2</version>
    <diagnostics>
      <diag:diagnostic>
      <diag:uri>200832</diag:uri>
        <diag:details/>
        <diag:message>Mandatory parameter version was not provided</diag:message>
      </diag:diagnostic>
    </diagnostics>
</searchRetrieveResponse>
````


## Reference
For more information please see <a href="https://knowledge.exlibrisgroup.com/Alma/Product_Documentation/010Alma_Online_Help_%28English%29/090Integrations_with_External_Systems/030Resource_Management/190SRU_SRW_Search">Ex Libris SRU/SRW Search</a>
