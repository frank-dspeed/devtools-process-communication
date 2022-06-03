# devtools-process-communication
A Toolset for devtools-process-communication can be used per process pipe or secure websockets.


## Fundamentals
Every communication is serialized to UTF-8 because of the ECMAScript Standard Implementation Details.
a Binary Pipe is possible when you know enough about browser API's and the Internals but not directly via the devtools protocol.
Only File Handling API's are able to binary stream for example the fetch stream API is able to transfer a binary unmodifyed stream
for example into WebGPU or Audio Context anything that would benefit from directly Binary data transmission.

this lib implements the most fundamental stuff like IPC RPC 

there are existing tutorials for this but they are complicated and outdated as they do not use ES2022+ Methods

This can be seen as Puppeteer Successor as it aims to transform the Puppeteer Source into Something useable Maintainable.
