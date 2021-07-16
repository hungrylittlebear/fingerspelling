<html>
    <head>
    <title>Fingerspelling Hand</title>

  <link href="http://fonts.googleapis.com/css?family=Source+Sans+Pro:200,400,700,400italic,700italic" rel="stylesheet" type="text/css">

  <style>
    * {
      margin: 0;
      padding: 0;
    }

    body {
      background: white;
      color: #333333;
      -webkit-font-smoothing: antialiased;
      font-size: 16px;
      font-family: "Source Sans Pro", Helvetica;
    }

    img {
      display: block;
    }

    em {
      font-size: 12px;
    }

    #signature {
      margin-left: 30px;
      font-style: oblique;
    }

    a:link,
    a:visited {
      color: #165788;
      text-decoration: none;
    }

    a:hover,
    a:focus,
    a:active {
      text-decoration: underline;
    }

    .wrapper {
      width: 660px;
      margin: auto;
    }

    .container {
      width: 660px;
      margin: auto;
    }

    #content {
      width: 650px;
      margin: 70px auto 0px auto;
    }

    #content article {
      margin-bottom: 150px;
    }

    #content h1,
    #content h2 {
      color: black;
      margin-bottom: 30px;
      font-weight: 200;
      font-size: 48px;
    }

    #content h3 {
      color: black;
      border-bottom: 1px solid black;
      text-transform: uppercase;
      margin: 30px 0px 30px 0px;
      font-size: 28px;
      font-weight: 200;
    }

    #content p {
      width: 100%;
      line-height: 150%;
      margin-bottom: 20px;
    }

    #content p:first-child {
      font-size: 18px;
      font-style: italic;
      letter-spacing: 2px;
    }

    #content p:first-child:first-line {
        font-weight: bold;
    }

    pre {
      font-size: 10px;
      padding: 15px;
      border-radius: 10px;
      background: #ddd;
    }
  </style>
</head>
<body>
  <div class="wrapper">
    <section id="content">
      <h1>Fingerspelling Hand</h1>
	  <h4>Connor Batch - CPE 471 - Winter 2015 - Zoe Wood</h4>
      <article>

		<h3>Project Description</h3>

        <p>This project entails a modeled hand capable of fingerspelling, specifically in American Sign Language (ASL).
           Every alphabetic key has been modeled, including double letters which can be accomplished through a sliding
           motion in ASL, and the letters which are modeled through a motion rather than simply a hand position (J and Z).</p>
		<center>
          <a>
              <img src="REST.PNG" width="100%">
          </a>
          <em>hand at rest</em>
        </center>

        <h3>How it Works</h3>

        <h4>What is a hand position?</h4>
        <p>There are several ways that a hand position could be modeled, similarly to how a human hand works, I decided
           that a hand could solely be modeled as a series of joint rotations. Each letter now can now be created through
           modifying the same underlying model, but providing different rotational values.</p>

		<center>
          <a>
              <img src="I.PNG" width="100%">
          </a>
          <em>the letter I</em>
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
