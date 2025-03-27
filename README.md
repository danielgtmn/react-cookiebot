# React Simple Cookiebot Consent Banner Loader

The Cookiebot Consent Banner Loader is a streamlined script designed to effortlessly integrate the Cookiebot consent management platform into your website. This lightweight, GDPR-compliant solution ensures that your site adheres to international privacy regulations by managing and documenting visitor consents for cookies and tracking technologies. Easy to implement and operate, the Cookiebot Loader enhances user trust by providing clear options to accept or reject cookies, maintaining a balance between compliance and user experience.
## Features

- Easy Integration
- Cookiebot Cookie Notifikation

## Installation

Install  with npm

```bash
  npm i @danielgtmn/react-cookiebot
```

## Usage/Examples
Create a Account at https://admin.cookiebot.com/ 

Get Your Implementation script and use only the data-cbid.
User this ID and set it as CookieBotID.

###  !! Only Works on Website registerd at Domains in Cookiebot Pannel !!

In the Main Layout File
Replace GTag with your GTag ID and GAnalytics with your Analytics Id

```javascript
import CookieBotLoader from "@danielgtmn/react-cookiebot";

function App() {
  return (
      <html lang="en">
            <body>
                <CookieBotLoader/>
                {children}
            </body>
        </html>

  )
}
```

## Options
Set in your .env File

| Option | Type     | Description            | Default   |
|--------|----------|------------------------|-----------|
| COOKIEBOT_ID | `string` | The ID of your Domain  | `""`      |
| COOKIEBOT_DEBUG | `string` | Enable the Debug Mode  | `"false"` |
| COOKIEBOT_URL | `string` | The URL from Cookiebot | `"https://consent.cookiebot.com/uc.js"` |
## Roadmap

- More Config Options

## License

[MIT](https://choosealicense.com/licenses/mit/)
