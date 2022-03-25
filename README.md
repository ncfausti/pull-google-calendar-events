# google calendar events starter project

## Prerequisites:
### Google Cloud Console Setup
1. Create a **PROJECT** on https://console.cloud.google.com/.
    1. Take note of the **API KEY** as you will need this later in your JS code.
2. On the sidebar, click **Credentials**.
3. Create a new **OAuth 2.0 Client ID** for **web**.
    1. Take note of the **CLIENT ID** as you will need this later in your JS code.
    2. Under <span style="color:#cc0000">**Authorized JavaScript origins**</span> add the following URI using the **ADD URI** button: http://localhost:8000 (for testing)
    3. Under <span style="color:#cc0000">**Authorized Redirect URIs**</span> add the following URI using the **ADD URI** button: http://localhost:8000 (for testing)
4. In the current directory (where index.html is located) start a web server on port 8000 using the following command for **python 3**:

    ```python3
    python3 -m http.server 8000
    ```
--- 

## Configure & Run

### Configure
Using the **CLIENT ID** and **API KEY** noted above, replace the values for each at lines 20 & 21 to use your specific values.

### Run

Visit http://localhost:8000 in your browser. 

When you click the **Authorize** button on that page, Google will attempt to log you in to your Google Calendar account. If successfull, you should be redirected back to http://localhost:8000 and your upcoming events should be displayed there.

Congratulations! You've successfully setup a starter app for Google Calendar API.