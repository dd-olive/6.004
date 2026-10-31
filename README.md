View course online at: [https://computation-structures.github.io/course](https://computation-structures.github.io/course)

You can view this course material using just your computer, i.e., no
internet access required after the initial setup.

* clone this repository onto your local computer.  Also install <a href="https://www.python.org/downloads/">python3</a> on your computer.

* change to directory where you cloned the repo.

* execute `python3 -m http.server` to start a local HTTP server listening on port 8000.

* browse to <a href="http://localhost:8000/">http://localhost:8000/</a> to see the
top-level webpage for the course.

You can compile the course material into a client/server grading model by running `make` in the top-level directory of the repository. This will generate the student files in the `_build` directory and the server files in the `_server` directory. If you serve the `_build` directory so that those files are accessible client-side and host the grading code at the same endpoint, but port n+1, students will be able to submit their work and receive grades from the server without exposing answers to easy scraping.

The purpose of the moving to a client-server model is that it forces cheaters to do an extra step to obtain the correct answers, making it less tempting to cheat one's way out of a deadline. If they need to give an AI access to the internet or a course bible in order to get answers, that is more extreme than clicking "view source" on a static webpage. As the future gets more futuristic, asking an AI for help with parts of a question will probably be as common as using a calculator for arithmetic today, and the chances that an AI accidentally cheats or explains something with fauty logic are lower if there are more barriers than hiding the answer in an HTML tag.
