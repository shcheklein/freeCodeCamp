---
id: 587d824c367417b2b2512c4d
title: Compare the Properties of Two Elements
challengeType: 2
forumTopicId: 301588
localeTitle: Сравните свойства двух элементов
---

## Description
<section id='description'>
Напомним, что этот проект строится на следующем стартовом проекте <a href="https://glitch.com/#!/import/github/freeCodeCamp/boilerplate-mochachai/">Glitch</a> или клонируется из <a href="https://github.com/freeCodeCamp/boilerplate-mochachai/">GitHub</a> . .isAbove () =&gt; a&gt; b, .isAtMost () =&gt; a &lt;= b
</section>

## Instructions
<section id='instructions'>
Use <code>assert.isAbove()</code>(i.e. greater) or <code>assert.isAtMost()</code> (i.e. less than or equal) to make the tests pass.
</section>

## Tests
<section id='tests'>

```yml
tests:
  - text: All tests should pass
    testString: getUserInput => $.get(getUserInput('url') + '/_api/get-tests?type=unit&n=7').then(data => {assert.equal(data.state,'passed'); }, xhr => { throw new Error(xhr.responseText); })
  - text: Choose the right assertion - isAbove vs. isAtMost
    testString: getUserInput => $.get(getUserInput('url') + '/_api/get-tests?type=unit&n=7').then(data => {  assert.equal(data.assertions[0].method, 'isAtMost', '5 is at most (<=) 5'); }, xhr => { throw new Error(xhr.responseText); })
  - text: Choose the right assertion - isAbove vs. isAtMost
    testString: getUserInput => $.get(getUserInput('url') + '/_api/get-tests?type=unit&n=7').then(data => {  assert.equal(data.assertions[1].method, 'isAbove', '1 is greater than 0'); }, xhr => { throw new Error(xhr.responseText); })
  - text: Choose the right assertion - isAbove vs. isAtMost
    testString: getUserInput => $.get(getUserInput('url') + '/_api/get-tests?type=unit&n=7').then(data => {  assert.equal(data.assertions[2].method, 'isAbove', 'Math.PI = 3.14159265 is greater than 3'); }, xhr => { throw new Error(xhr.responseText); })
  - text: Choose the right assertion - isAbove vs. isAtMost
    testString: getUserInput => $.get(getUserInput('url') + '/_api/get-tests?type=unit&n=7').then(data => {  assert.equal(data.assertions[3].method, 'isAtMost', '1 - Math.random() is > 0 and <= 1. It is atMost 1 !'); }, xhr => { throw new Error(xhr.responseText); })

```

</section>
