<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style>
@import "./common/font/font.css";
html,
body,
div,
span,
h1,
h2,
h3,
h4,
h5,
h6,
p,
a,
em,
img,
small,
strike,
strong,
b,
u,
i,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
figure,
figcaption,
footer,
header,
hgroup,
main,
menu,
nav,
section,
summary,
audio,
video {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
  box-sizing:border-box;
  font-weight: normal;
}

/* HTML5 display-role reset for older browsers */
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
main,
menu,
nav,
section {
  display: block;
}

input,
button {
  border: none;
  outline: none;
}

*[hidden] {
  display: none;
}

ol,
ul {
  list-style: none;
}

blockquote,
q {
  quotes: none;
}

blockquote:before,
blockquote:after,
q:before,
q:after {
  content: "";
  content: none;
}

table {
  border-collapse: collapse;
  border-spacing: 0;
}

html,
body {
  height: 100%;
  width: 100%;
  font-size: 12px;
  color: #323B37;

}

</style>
