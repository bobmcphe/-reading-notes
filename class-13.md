# Class 13 Reading Notes

## Local Storage
HTML5 has sought to fix many issues and to provide some consolidation. Dealing with persistant data is one of those. Local storage, called by the author HTML storage, is a new solution here to stay, it sounds like. The max if 5mb, far more than the 4k that cookies provide, but far less than what a database can provide. This 5mb is for each origin, and will throw an error if the limit is exceeded. It is also worth noting that the storage can be increased by the user, but only by the user, there is no way for any outside party to request an increase, and even then, only some browsers provide this user-controlled capability (e.g. Opera).

Local Storage is, "Simply put,...a way for web pages to store named key/value pairs locally, within the client web browser." It also works on key/value pairs, but these key/value pairs are always converted to a string in order to be stored. Therefore, it must be de-converted, so to speak. The four main functions that are used with this are:

1. setItem(); to create an item
1. getItem(); to access an item
1. setItem(); to override the item created
1. removeItem(); to delete a key/value pair

However, some people would like to see the key/value method of storing data become obsolete, using for example Web SQL Database or IndexedDB.