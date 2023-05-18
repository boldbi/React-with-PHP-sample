# BoldBI Embedding React with PHP Sample

 This Bold BI React with PHP sample contains the dashboard embedding samples.In this sample, `React` application act as the front-end, and `PHP` acts as the back-end application. This sample demonstrates the rendering of dashboard available in your Bold BI server.

This section guides you in using the Bold BI dashboard in your React with PHP sample application.

 * [Requirements to run the demo](#requirements-to-run-the-demo)
 * [Using the React with PHP sample](#using-the-react-with-php-sample)
 * [Online Demos](#online-demos)
 * [Documentation](#documentation)

 ## Requirements to run the demo

The samples require the following requirements to run.

 * [PHP installer](https://windows.php.net/download/)
 * [Node.js](https://nodejs.org/en/)
 * [Visual Studio Code](https://code.visualstudio.com/download)
 * In Visual studio code download the extensions, PHP intelephense and PHP Server.

 ## Using the React with PHP sample
 
 * Open the PHP sample in visual studio code or any respective IDE.
 
 * Open the `authorizeserver.php` in the location, /PHP/rest/authorizeserver.php and provide the mandatory values as per your Bold BI Server.
 
 <meta charset="utf-8"/>
    <table>
    <tbody>
        <tr>
            <td align="left">UserEmail</td>
            <td align="left">UserEmail of the Admin in your Bold BI, which will be used to get the dashboards .</td>
        </tr>
        <tr>
            <td align="left">secretCode</td>
            <td align="left">Get your EmbedSecret key from the Embed tab by enabling the Enable embed authentication in the [administration page](https://help.boldbi.com/embedded-bi/site-administration/embed-settings/).</td>
        </tr>
    </tbody>
    </table>
	
 * Now, run the PHP sample.

 * Open the React sample in Visual studio code.

 * Open the `DashboardListing.js` file in the following location, /src/DashboardListing/DashboardListing.js.

 * Please change the following properties in the `DashboardListing.js` file as per your Bold BI Server.

    <meta charset="utf-8"/>
    <table>
    <tbody>
        <tr>
            <td align="left">apiHost</td>
            <td align="left">PHP application would be run on http://localhost:3000/, which needs to be set as apiHost.</td>
        </tr>
        <tr>
            <td align="left">RootUrl</td>
            <td align="left">Dashboard Server URL (Eg: http://localhost:5000/bi, http://demo.boldbi.com/bi).</td>
        </tr>
        <tr>
            <td align="left">SiteIdentifier</td>
            <td align="left">For the Bold BI Enterprise edition, it should be like `site/site1`. For Bold BI Cloud, it should be an empty string.</td>
        </tr>
        <tr>
            <td align="left">Environment</td>
            <td align="left">Your Bold BI application environment. (If Cloud, you should use `cloud,` if Enterprise, you should use `enterprise`).</td>
        </tr>
        <tr>
            <td align="left">authorizationUrl</td>
            <td align="left">Url of the 'GetDetails' action in the PHP application.</td>
        </tr>
        <tr>
            <td align="left">dashboardId</td>
            <td align="left">Dashboard Id of dashboard you want to embed.</td>
        </tr>
    </tbody>
    </table>

* Now run the React sample.

### Install npm

To install all dependent packages, use the below command

```bash
npm install
```

### Run/Serve

To run the sample, use the below command

```bash
npm start
```

<!-- Commanded the below line, since help documentation is not available for this sample. Once crated need to update the hyperlink -->
<!-- Please refer to the [help documentation]() to know how to run the sample. -->

## Online Demos

Look at the Bold BI Embedding sample to live demo [here](https://samples.boldbi.com/embed).


## Documentation

A complete Bold BI Embedding documentation can be found on [Bold BI Embedding Help](https://help.boldbi.com/embedded-bi/javascript-based/).