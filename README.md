Clone project and then
* enter to directory with project
* run: ```spring boot```

enter to directory ```src/main/resources```
and generate self signed certificate (in repository certificate might be expired):
```bash
keytool -genkey -alias tomcat -keyalg RSA  -keystore keystore.jks
```

```
How to use:
1.Create a room
2. The interlocutor should join the room
3. Exit the room you can by pressing the button 'leave'
```

then:
* run: ```spring boot ```
* enter [https://localhost:8445](https://localhost:8445) in your favourite browser
(**HTTPS is important, because default http handler isn't configured**)
* accept untrusted certificate

_Sometimes websocket (js side) is throwing exception then try to change localhost to 127.0.0.1_
