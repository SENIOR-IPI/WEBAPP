## Senior-IPI calculator : Web APP

A public acccess to the Senior IPI calculator is available as a <a href="https://senior-ipi.netlify.app" target="_blank">Web App</a>.

Local versions of Senior IPI calculator can also be installed on a computer or an intranet server. The Senior-IPI calculator needs only an http daemon to launch the web app. Note that the web app works only in the browser environment and no further interaction (cookies, remote execution...) exists with the server after launching the web app.

### Installation of the Senior-IPI calculator with a local http daemon

- Download the [calculator archive](https://github.com/SENIOR-IPI/WEBAPP/blob/main/webapp.zip "Senior-IPI Web APP") and extract it to a directory.

- A simple way to launch the web app is to use the Python integrated http daemon. In the command line, navigate to the web app's directory and run the command:

  ```         
  python3 -m http.server
  ```

- Any http server can be used (apache, nginx, nodejs...). Note that the calculator directory needs to be defined as the root of the web site. A workaround to integrate the calculator for example in an intranet is to launch it in an <a href="https://www.w3schools.com/tags/tag_iframe.ASP" target="_blank">iframe</a>.
