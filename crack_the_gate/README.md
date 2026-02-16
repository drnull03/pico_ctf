
---


After visiting the website and checking the HTML source code using **Ctrl+U**, I found the following comment:

```html

<!-- ABGR: Wnpx - grzcbenel olcnff: hfr urnqre "K-Qri-Npprff: lrf" -->
<!-- Remove before pushing to production! -->  
```

### Identification

I suspected the string was encoded with **ROT13**. To confirm, I used the [dCode Cipher Identifier](https://www.dcode.fr/cipher-identifier), which verified it was indeed ROT13.

### Decoding

After using an online tool like [rot13.com](https://rot13.com/), I obtained the following note:

> **NOTE:** Jack - temporary bypass: use header "X-Dev-Access: yes"

### Final Step

To retrieve the flag, I injected the discovered string as an HTTP header using burp suite. Although There are several ways to accomplish this other than burp:

* **Browser Developer Tools:** Use the Network tab to edit and resend the request with the new header.
* **cURL:** This is often the most efficient method. You can add the header using the following command:

```bash
curl -H "X-Dev-Access: yes" [URL]

```

---

