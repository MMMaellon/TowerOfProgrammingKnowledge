---
title: The Tower
# date: 2024-01-08T05:07:55-08:00
draft: false
---

{{<hidden id="asdf">}}

![image](https://images.unsplash.com/photo-1534415378365-701353a65fed?q=80&w=720&h=800&auto=format&fit=crop&crop=bottom&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D#center)

{{</hidden>}}

{{<terminal id="term" >}}
ascend: function() {
    this.echo('Hello, user. Welcome to this terminal.', {typing: true, delay: 50});
}
{{</terminal>}}


<script>
async function animation(){
    $('#asdf').addClass("fade-in-slow");
    $('#asdf').removeClass("hidden");
    term.focus(true);
    await term.echo("[[g;white;]The Tower of Programming Knowledge]", { typing: true, delay: 50, keepWords: true } );
    await term.echo("----------------------------------\nThis tower shares with all who ask the knowledge needed to make his or her first programming journey.", { typing: true, delay: 2, keepWords: true } );
    await term.echo("\nAll it asks for in return is your determination to reach its peak.", { typing: true, delay: 2, keepWords: true } );
    await term.echo("\nEnter your name to proceed.", { typing: true, delay: 50, keepWords: true } );
    term.read(">> ").then(async (name) =>{
        await term.set_prompt("\nBe welcomed to this place, [[g;white;]" + name + "].", {typing: true, delay: 50, keepWords: true});
        term.freeze(true);
        await sleep(1000);
        window.location.href = '/TowerOfProgrammingKnowledge/next';
    });
    // term.freeze(true);
}

animation()
</script>

<!-- <script src="terminal.js"></script> -->
<!-- <script src="terminal.css"></script> -->
<!-- <div class="tv"> -->
<!--     <div class="collection external terminal"> -->
<!--         See Also: <a href="https://codepen.io/jcubic/pen/JjpzzOr" target="top">Red version</a>, or <a href="https://codepen.io/collection/AeGGxz" target="top">Vintage Screen Effects</a>, <a href="https://codepen.io/collection/Mgrkmw"  target="top">Terminal Things</a>, and <a href="https://codepen.io/collection/LPjoaW" target="top">other jQuery Terminal demos</a>. -->
<!--     </div> -->
<!--     <div class="flicker"></div> -->
<!--     <div class="scanlines"></div> -->
<!--     <div class="noise"></div> -->
<!-- </div> -->

