# discord webhook sender

welcome to the **discord webhook sender**, also known as the highly advanced, extremely sophisticated, definitely-not-goofy webpage for sending messages to discord.

this thing does basically one job:

**you type words → you click send → discord receives the words.**

revolutionary technology. absolutely groundbreaking.

## features

* send messages to discord webhooks
* add multiple webhook apis
* give each api a name
* remove apis you no longer need
* saves webhook settings locally in your browser
* clear the message box
* simple api configuration page
* dark mode because obviously
* sends messages directly through discord's webhook api
* no database
* no complicated backend
* no giant enterprise dashboard
* just html, css, javascript, and questionable amounts of confidence

## how it works

first, configure a discord webhook.

then give it a name.

then paste the webhook url.

then save it.

then go back to the main page.

then type your message.

then press **send**.

and boom.

the message has left the building.

```text
you
 |
 | types message
 v
webhook sender
 |
 | sends request
 v
discord
 |
 v
message appears
```

## api configuration

the settings page lets you store multiple webhook configurations.

for example:

```text
main server
test server
the goofy server
definitely-not-the-test-server
probably-the-main-server
```

each one can have its own webhook url.

you select whichever one you want before sending a message.

## local storage

your configured webhooks are stored using your browser's `localstorage`.

this means the webpage can remember your settings after you refresh it.

basically:

```text
browser: "i remember your webhook"

you: "thanks bro"

browser: "you're welcome"
```

the webpage itself does not need a database to store the configurations.

however, webhook urls should still be treated like secrets. don't casually paste them into random computers or publish them online.

## sending messages

the sender uses a normal http post request with json.

the message is sent like this:

```json
{
  "content": "your extremely important message"
}
```

discord then decides whether it wants to accept the request.

if everything works:

```text
message sent!
```

if something goes wrong:

```text
discord returned http 400
```

or perhaps:

```text
error: something exploded
```

very useful. extremely professional.

## clear button

the clear button does exactly what it says.

you click it.

the message disappears.

the status goes back to:

```text
ready.
```

no complicated process.

just gone.

## why does this exist?

because sometimes opening discord, finding the correct channel, typing the message, and pressing enter is apparently too much work.

so instead we created:

**the message yeeter 9000**

is it necessary?

probably not.

is it useful?

sometimes.

is it goofy?

absolutely.

## don't spam

please don't use this to absolutely destroy a discord server with thousands of messages.

discord has rate limits, and repeatedly sending requests can cause them to be rejected.

also, nobody wants this appearing in their server:

```text
hello
hello
hello
hello
hello
hello
hello
hello
hello
hello
```

that's not communication.

that's psychological warfare.

use it for normal webhook messages and testing instead of flooding your server.

## webhook safety

treat webhook urls like passwords.

don't post them publicly.

don't put them in screenshots.

don't commit them to github.

don't send them to random people.

if somebody gets your webhook url, they may be able to send messages through that webhook.

if a webhook gets leaked, delete or rotate it from discord and create a new one.

## technologies

this project uses the ancient and powerful stack:

* html
* css
* javascript
* localstorage
* discord webhooks
* pure browser technology
* approximately zero quantum computers

no massive framework.

no 48 npm packages.

no kubernetes cluster.

no blockchain.

just javascript doing javascript things.

## project structure

the entire thing can live inside one html file:

```text
discord-webhook-sender/
└── index.html
```

that's it.

one file.

one webpage.

one questionable amount of power.

## example setup

you could configure:

```text
api name:
main server

webhook url:
https://discord.com/api/webhooks/...
```

then select:

```text
main server
```

type:

```text
hello from the goofy webhook machine
```

and press:

```text
send
```

discord:

```text
message received
```

you:

```text
nice
```

## if something breaks

don't panic.

check these things first:

1. make sure the webhook url is correct
2. make sure the webhook still exists
3. make sure the message isn't empty
4. make sure your internet connection works
5. check the status message
6. check the http status returned by discord
7. try refreshing the page
8. if none of that works, stare at the code for 15 minutes and pretend you're debugging

classic developer workflow.

## disclaimer

this project is intended for normal and reasonable webhook usage.

please don't use it to spam, harass, disrupt, or otherwise annoy people.

use your webhook powers responsibly.

with great webhook comes great responsibility.

## conclusion

congratulations.

you now have a webpage that can:

**type message**

↓

**click button**

↓

**discord gets message**

this may not change the world.

but it does send messages to discord.

and honestly?

that's enough.

**discord webhook sender**

*powered by javascript, localstorage, and questionable decisions.*
