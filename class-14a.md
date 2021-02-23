# Read: 14a - CSS Transforms, Transitions, and Animations
## What Google Learned From Its Quest to Build the Perfect Team
* ‘We had lots of data, but there was nothing showing that a mix of specific personality types or skills or backgrounds made any difference. The ‘‘who’’ part of the equation didn’t seem to matter.’
* ‘As long as everyone got a chance to talk, the team did well. But if only one person or a small group spoke all the time, the collective intelligence declined.’
## CSS Transforms
#### 2D Transforms
1. 2D Rotate::
The rotate value provides the ability to rotate an element from 0 to 360 degrees. 
`.box-1 {
  transform: rotate(20deg);
}`
2. 2D Scale::
Using the scale value within the transform property allows you to change the appeared size of an element.
`.box-2 {
  transform: scale(1.25);
}
`
#### CSS Transitions & Animations
1. Transitions::
for a transition to take place, an element must have a change in state, and different styles must be identified for each state.
`.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}
`
#### 8 simple CSS3 transitions that will wow your users
1. Fade in
`.fade
{
        opacity:0.5;
}
.fade:hover
{
        opacity:1;
}
`
2. Change color
`.color:hover
{
        background:#53a7ea;
}`
3. Grow & Shrink
`.grow:hover
{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
}`


