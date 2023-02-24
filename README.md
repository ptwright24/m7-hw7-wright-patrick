# m7-hw7-wright-patrick



/* tooltip code below */

span.tooltip {
  color: var(--danger-color);
  position: relative;
  cursor: pointer;
}

/* underline span on hover/focus */
span.tooltip:hover,
span.tooltip:focus {
  text-decoration: underline;
  position: relative;
}
/* show tooltip on hover/focus */
span.tooltip:hover > span,
span.tooltip:focus > span {
  display: inline;
  visibility: visible;
}

/* styling for tooltip bubble */
span.tooltip span {
  display: none;
  visibility: hidden;
  width: 120px;
  background-color: black;
  color: white;
  text-align: center;
  padding: 5px 0;
  border-radius: 6px;
}

/* styling for tooltip bubble arrow */
span.tooltip span::after {
  content: "";
  position: absolute;
  top: 100%;
  left: 50%;
  margin-left: -5px;
  border-width: 5px;
  border-style: solid;
  border-color: black transparent transparent transparent;
}