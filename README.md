# Fingerspelling Hand
Connor Batch - CPE 471 - Winter 2015 - Zoe Wood</h4>


## Project Description
This project entails a modeled hand capable of fingerspelling, specifically in American Sign Language (ASL). Every alphabetic key has been modeled, including double letters which can be accomplished through a sliding motion in ASL, and the letters which are modeled through a motion rather than simply a hand position (J and Z).

<img src="REST.PNG" width="100%">

## How it WOrks

### What is a hand position?
There are several ways that a hand position could be modeled, similarly to how a human hand works, I decided that a hand could solely be modeled as a series of joint rotations. Each letter now can now be created through modifying the same underlying model, but providing different rotational values.</p>

<img src="I.PNG" width="100%">
the letter I
        </center>

        <h4>The Buffer</h4>
        <p>As the user types, the keys they enter are being pushed into a queue that will constantly be updating on the
           screen as long as the queue isn&#39;t empty. This allows the user to type out a full sentence and the hand will not
           jump between signs, it will spell them out in the order that they typed in.</p>

        <h4>Motion</h4>
        <p>Movement occurs when there is another item ready to be signed in the queue. The current hand position becomes
           the new starting position and the destination is the next letter to be signed. The current hand position is then
           updated between the two positions until it arrives at the destination.</p>
        <p> The speed in which the hand is fingerspelling is variable and can be modified with the UP and DOWN arrow keys.</p>

        <h3>See it in Action</h3>
          <p>A demonstration of how movement is modeled through the progression throughout the entire alphabet is shown below.</p>
		<center>
          <a>
              <img src="alpha.gif" width="100%">
          </a>
          <em>ASL alphabet</em>
        </center>

        <p>There are two special cases to make note of and both are covered with the following demonstration of "hello world".
           First is spaces - a space is used deliminate between words, which is characterized in ASL with a pause on the last
           letter. The second is a double-letter, this is accomplished in ASL with a slide. Both have been accounted for and
           are available to be witnessed below.</p>
		<center>
          <a>
              <img src="hello_world.gif" width="100%">
          </a>
          <em>"hello world"</em>
        </center>

        <h3>Future Work</h3>
        <p>My mom and her half of my family are Deaf, which is why I&#39;m fluent in ASL and was motivated to take on this project.
           A future goal could be for educational usage. There are ASL classes that are dedicated entirely to fingerspelling,
           if I could implement this on a website using WebGl then it could be a fun easy tool for those who are learning and
           want to practice their comprehension at faster or slower speeds.
           </p>

      </article>
    </section>
  </div>

</body></html>
