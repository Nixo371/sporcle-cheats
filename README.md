# sporcle-cheats
Sporcle is a joke

Run this snippet in slideshow-type quizzes in Sporcle and watch as your computer takes the quiz for you:
```
let loop_variable = 0;
let question_amount = [insert amount of questions];

let loop = setInterval(( function () {
    if (loop_variable == question_amount) { clearInterval(loop) }
    for (let j = 0; j < question_amount; j++) {
        document.getElementById("gameinput").value = getAnswer(j);
        checkGameInput(document.getElementById("gameinput"));
    }
    loop_variable++;
}
), 2000);
```
