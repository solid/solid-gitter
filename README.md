# solid-gitter
A command line or batch processing tool to move data from [gitter](https://gitter.im)
chat into a [solid](https://solid.inrupt.net/) pod.

Do you have a projects which use gitter chats, but you would like to do do soli things
with them, like bookmark chat messages, and so on?
Do you have a lot of your projects institutional memory in gitter chats, and worry about
it gitter going away one day, or being offline?  Do you want to be able to use and build all kinds of search and
analysis tools on top of your gitter chat data?  Maybe you should be using this script.


## Usage
### Solid access

You will need to give your script access to solid account which will have write access
to the pod where you will be storing the solid chat.

### Gitter access

You will need to give the script access to the gitter world, which means to get a gitter token.
See https://developer.gitter.im/docs/welcome   .

[Get a token](https://developer.gitter.im/apps).

Then you can save it and pass it to this program as an environment variable.

Syntax for example:
```
export GITTER_TOKEN=W4gfhEf6XO4+p1bfTEHy3ncEVDUTksI2pYMryWhO4ZbhQrq2229Bm
node gitter-solid.js   list

```
One you have set your shell session up with the gitter token,
you can use gitter-solid repeatedly.

## Gitter rooms

In gitter, the concept of a room includes public rooms, private rooms, and private 1-1 conversations, some call *direct messaging*.

 | `node gitter-solid.js list` | List your gitter rooms |
 | `node gitter-solid.js list public` | List your public rooms |
 | `node gitter-solid.js list private` | List your private rooms |
 | `node gitter-solid.js list direct` | List your direct messaging 1:1 chats |
