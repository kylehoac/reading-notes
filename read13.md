# Reading Notes 13 Course 201

__*What is HTML5 Storage (local storage)*__
HTML5 Storage, commonly referred to as local storage, is a way for web pages to store key/value pairs locally within the web browser. This data persists even after navigating off of the website, closing the time, or closing the browser.

- Faster than cookies since it doesn't have to transmit data to the web browser
- Most web browsers support HTML5
- Works by retrieving data from the key, and returning that key's value

The data stored inside of local storage is stored as a string. Before storing data you must stringify the data and give it a label, then set it in the local storage.

To retrieve data within the local storage you must parse the data to turn it back into its previous JS data type.

> calling setItem() with a named key that already exists will overwrite its previous value
>> Calling getItem() with a non existent key will return null

To remove a key you can use:

> removeItem();

To keep track of when a storage area changes, you can trap it within the storage event. Storage events are fired off whenever setItem(), removeItem(); or clear() is called.

[<== Back to Main Page](README.md)
