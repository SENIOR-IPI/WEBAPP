## SENIOR-IPI calculator : Web APP

A public access to the Senior IPI calculator is available as a <a href="https://senior-ipi.netlify.app" target="_blank">Web App</a>. Note that the web app has been optimized to work on ios and android browsers .

Local versions of Senior IPI calculator can also be installed on a computer or an intranet server. The Senior-IPI calculator needs only an http daemon to launch the web app. Note that the web app works only in the browser environment and no further interaction (cookies, remote execution...) exists with the server after launching the web app.

### Installation of the Senior-IPI calculator with a local http daemon

- Download the [calculator archive](https://github.com/SENIOR-IPI/WEBAPP/blob/main/webapp.zip "Senior-IPI Web APP") and extract it to a directory.

- A simple way to launch the web app is to use the Python integrated http daemon. In the command line, navigate to the web app's directory and run the command:

  ```         
  python3 -m http.server
  ```

- Any http server can be used (apache, nginx, nodejs...). Note that the calculator directory needs to be defined as the root of the web site. A workaround to integrate the calculator for example in an intranet, is to launch it in an <a href="https://www.w3schools.com/tags/tag_iframe.ASP" target="_blank">iframe</a>.Installation of the Senior-IPI calculator with the `SeniorIPIWeb` R package

### Installation of the `SeniorIPIWeb` R package

An R package is also available to launch the web app in an R environment.

- Download either the binary [Windows R](https://github.com/SENIOR-IPI/WEBAPP/blob/main/SeniorIPIWeb_0.1.0.zip) or the [source](https://github.com/SENIOR-IPI/WEBAPP/blob/main/SeniorIPIWeb_0.1.0.tar.gz) package for the other operating systems.

- Install the source or windows package from a R session:

  - Windows package

    ``` r
    install.packages("<path to the download folder>/SeniorIPIWeb_0.1.0.zip")
    ```

  - Source package

    ``` r
    install.packages("<path to the download folder>/SeniorIPIWeb_0.1.0.tar.gz")
    ```

- Load the `SeniorIPIWeb` package

  ```
  library(SeniorIPIWeb)
  ```

The web app is automatically launched in a web page or in the RStudio viewer and this type of message appears in the console :

```         
To stop the server, run servr::daemon_stop(1) or restart your R session.
Serving the directory \<R library path>\SeniorIPIWeb\webapp at http://127.0.0.1:4321
```

Note that the `SeniorIPIWeb` package depends on the `servr` package. The latter will be installed automatically upon first loading `SeniorIPIWeb.`
