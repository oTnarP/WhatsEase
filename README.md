### `README.md`  

```md
# WhatsEase - WhatsApp Live Chat Plugin   

WhatsEase is a lightweight JavaScript plugin that enables website owners to integrate a live chat button for WhatsApp. With WhatsEase, visitors can directly chat with businesses on WhatsApp with just one click.  

## 🚀 Features

- Simple one-step integration with any website.  
- Customizable chat button (color, text, logo, position).  
- Auto-show feature for instant visibility.  
- Responsive design for mobile and desktop.  
- No database or backend required.  

## 📌 Installation  

### Step 1: Add JavaScript File  
Download or include the `whatsEaseWidget.js` file in your website’s JavaScript folder.  

<script>
    var url = 'js/whatsEaseWidget.js';
    var s = document.createElement('script');
    s.type = 'text/javascript';
    s.async = true;
    s.src = url;

    var options = {
        "enabled": true,
        "chatButtonSetting": {
            "backgroundColor": "#00e785",
            "ctaText": "Chat with us",
            "borderRadius": "25",
            "marginLeft": "0",
            "marginRight": "20",
            "marginBottom": "20",
            "ctaIconWATI": true,
            "position": "right"
        },
        "brandSetting": {
            "brandName": "Your Brand",
            "brandImg": "logo.png",
            "welcomeText": "Hello! How can we assist you?",
            "messageText": "Hi, I need help!",
            "backgroundColor": "#00e785",
            "phoneNumber": "YourWhatsAppNumberWithoutPlus"
        }
    };

    s.onload = function () {
        CreateWhatsappChatWidget(options);
    };

    var x = document.getElementsByTagName('script')[0];
    x.parentNode.insertBefore(s, x);
</script>
```

### Step 2: Place Code Before `</body>`  
Ensure you place the above script **before** the closing `</body>` tag of every page where you want the chat button to appear.  

---

## 🎨 Customization  

You can modify the `options` object to change the appearance and behavior of the WhatsEase widget.  

### Chat Button Settings  
| Property         | Description                        | Default Value |
|-----------------|----------------------------------|--------------|
| `backgroundColor` | Button background color | `#00e785` |
| `ctaText` | Call-to-action text on the button | `"Chat with us"` |
| `borderRadius` | Rounded edges (in pixels) | `25` |
| `position` | Button position (`right` or `left`) | `"right"` |
| `marginBottom` | Distance from bottom (px) | `20` |
| `marginRight` | Distance from right (px) | `20` |

### Brand Settings  
| Property         | Description                        | Default Value |
|-----------------|----------------------------------|--------------|
| `brandName` | Name displayed on chat box | `"WhatsEase"` |
| `brandImg` | Logo image file | `"logo.png"` |
| `welcomeText` | Welcome message in chat box | `"Hi there! How can I help you?"` |
| `messageText` | Default message when chat opens | `"Hello, I am looking for help!"` |
| `phoneNumber` | WhatsApp number (without `+`) | `"YourNumber"` |

---

## 📷 Screenshots  
![WhatsEase Screenshot](screenshot.png)  

---

## 🛠️ Compatibility  
✅ Works on all modern browsers (Chrome, Firefox, Edge, Safari).  
✅ Compatible with WordPress, HTML, PHP, and React websites.  

---

## 📝 License  
This project is free to use with no restrictions. You are welcome to use, modify, and distribute it as you see fit.  

---

## 🤝 Contributing  
Want to improve WhatsEase? Fork the repository and submit a pull request!  

---

## ⭐ Support  
If you find this project helpful, please give it a **star ⭐** on GitHub!  
```
