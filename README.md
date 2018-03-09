# fake_realdonaldtrump
This repo houses a data collection module to collect tweets from [Donald J. Trump](https://twitter.com/realdonaldtrump). These tweets are then stored in a MySQL database. The deep learning portion of the repo is a recurrent neural network (RNN) which uses the tweets collected from @realdonaldtrump for training.

## Notes
### Automated Scrolling
It appears that the below JavaScript code logs no elements (remove backslash from getElementsByTagName).
var htmle = document.getElementsByTagName("\*")
for (var i = 0; i < htmle.length; i++){
	if (htmle[i].scrollTop != 0)
		console.log(htmle[i], htmle[i].scrollTop);
};

Because of this, Twitter appears to be using some alternate way to scroll down the page, since all elements have a scrollTop (vertical scroll offset) of 0, regardless of the visible scrolled position on the page.
