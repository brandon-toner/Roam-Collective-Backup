- [Personas](https://www.rodrigofranco.com/roam-personas-css.html)
    - Examples
        - #[P:Self](<../P:Self.md>) Inner Self Talk
        - #[P:Loving](<../P:Loving.md>) Love thyself
        - #[P:Critic](<../P:Critic.md>) Hard on yourself
    - ```css
/***************/
/** personas **/
/**************/

[data-tag="P:Self"]{
  background: [DFDDD5](<../DFDDD5.md>);
  padding: 3px 10px 3px 10px;
  border-radius: 5px;
  position: relative;
  margin-right: 10px;
  color:black;
}

[data-tag="P:Loving"]{
  background: [e2d0cb](<../e2d0cb.md>);
  padding: 3px 10px 3px 10px;
  border-radius: 5px;
  position: relative;
  margin-right: 8px;
  color:red;
}

[data-tag="P:Critic"]{
  background: [C4CBB7](<../C4CBB7.md>);
  padding: 3px 10px 3px 10px;
  border-radius: 5px;
  position: relative;
  margin-right: 10px;
  color: brown;
}

[data-tag="P:Self"]:after {
	content: '';
	position: absolute;
	right: 0;
	top: 50%;
	width: 0;
	height: 0;
	border: 10px solid transparent;
	border-left-color: [DFDDD5](<../DFDDD5.md>);
	border-right: 0;
	border-bottom: 0;
	margin-top: -8px;
	margin-right: -10px;
}

[data-tag="P:Loving"]:after {
	content: '';
	position: absolute;
	right: 0;
	top: 50%;
	width: 0;
	height: 0;
	border: 10px solid transparent;
	border-left-color: [e2d0cb](<../e2d0cb.md>);
	border-right: 0;
	border-bottom: 0;
	margin-top: -8px;
	margin-right: -10px;
}

[data-tag="P:Critic"]:after {
	content: '';
	position: absolute;
	right: 0;
	top: 50%;
	width: 0;
	height: 0;
	border: 10px solid transparent;
	border-left-color: [C4CBB7](<../C4CBB7.md>);
	border-right: 0;
	border-bottom: 0;
	margin-top: -8px;
	margin-right: -10px;
}```
- 
