# Exchange-Files
## Distributed systems

### Goals
In the present work we intended to implement a platform for sharing music files in the form of client/server in Java using *sockets* and *threads*.

### Application
File exchange platforms like SoundCloud allow musicians to share their creations directly with their fans. For this purpose, they can upload music files accompanied by various meta-information (title, author, interpreter, genre, ...). Meta-information is used so that listeners are aware of shared files and can perform searches. Having found the desired files, they can then download them for later use.

Bearing in mind that the files to be exchanged are of considerable size, usually with several MB, the implementation of these systems has to pay particular attention to the resources consumed with the storage, manipulation and transmission of these files. In particular, it is important to limit the number of simultaneous operations that can be carried out in order not to overload the system and to maintain a relative fairness between the different users.

### Client & Server
A client has been made available that offers a user interface to support the developed features. This client was written in Java using TCP *threads* and *sockets*.

The server was also written in Java, using TCP threads and sockets, keeping in memory the information relevant to the developed characteristics (except the contents of the files themselves), receiving and input from clients, as well as reaching them the desired information. The protocol between client and server was text-based, line-oriented (except for the content of the files themselves). In order for the server not to be vulnerable to slow clients, each thread does not request more than one socket.

### Functionalities
* Authentication and User Registration
* Publish a Music File
* Perform a Music Search
* Download a music file
* Download Limit
* Notification of new songs
* Unlimited file size

## Team

![Gonçalo Pinto][grp-pic] | ![Nuno Costa][nuno-pic] | ![João Parente][parente-pic]
:---: | :---: | :---:
[Gonçalo Pinto][grp] | [Nuno Costa][nuno] | [João Parente][parente]

[grp]: https://github.com/GRP99
[grp-pic]: https://github.com/GRP99.png?size=120
[nuno]: https://github.com/jnuno420
[nuno-pic]: https://github.com/jnuno420.png?size=120
[parente]: https://github.com/Joao-Parente
[parente-pic]: https://github.com/Joao-Parente.png?size=120

<div align="center">
  <sub>September 2019 - January 2020</sub>
</div>