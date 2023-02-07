# Link extraction A-Z


# Requirements ... 
1. newPipe / org.schabi.newpipe
2. URLCheck / com.trianguloy.urlchecker
3. Visual Studio Code. || VSCode || VSC || (My fucking app.)


# Instructions ... 
1. Install these two apps on your android.
2. Configure these apps accordingly.
3. Open your internet connection.
4. Open newPipe.
5. Go to the respected channel where you wanted to copy links from.
6. Click on the "Play All" button. 
7. The first video will start playing.
8. Then click on the "playlist" button. 
9. Scroll through the list, untill you see the last video on the channel.
10. Then click on the add to playlist button.
11. Name your playlist.
12. Close that video.
13. Go to the "bookmark" section.
14. Find that playlist.
15. Click on that playlist.
16. At the top-right, there is a share button.
17. Click on that share button.
18. Share it to "URLCheck" app.
19. Now you will see all the links.
20. Copy all the links.
21. And save it in a txt file.
22. Im naming that as "raw-links-from-${}.txt"
23. You can name it whatever you want.
24. But dont modify that file.
25. Copy that file as 'new-to-old.txt'
26. Now we will modify that file.
27. Convert every line into a string, followed by a (, ) comma.
28. For this we are gonna use my fucking app.
29. Open my app. ( VSCode )
30. And start converting every link to a string followed by a comma.
31. Put that in an array.
32. Name that array.
33. Im naming that array as 'links'
34. create an html file.
35. paste this code.
```html
<!DOCTYPE html>
<html>
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>link-reverser</title>
	
</head>
<body>
	<h3 id="dumDum" ></h3>
	
	
	<script src="app.js"></script>
</body>
</html>
```
36. create a js file.
37. copy this code and 

```js

// grabbing stuff from dom
let dumDum = document.getElementById("dumDum");

// new to old links
// newest are at the top

let links = [
"https://www.youtube.com/watch?v=00000000001",
"https://www.youtube.com/watch?v=00000000002",
"https://www.youtube.com/watch?v=00000000003",
"https://www.youtube.com/watch?v=00000000004",
"https://www.youtube.com/watch?v=00000000005",
"https://www.youtube.com/watch?v=00000000006",
"https://www.youtube.com/watch?v=00000000007",
"https://www.youtube.com/watch?v=00000000008",
"https://www.youtube.com/watch?v=00000000009",
"https://www.youtube.com/watch?v=00000000010",
"https://www.youtube.com/watch?v=00000000011",
"https://www.youtube.com/watch?v=00000000012",
"https://www.youtube.com/watch?v=00000000013",
"https://www.youtube.com/watch?v=00000000014"
]

console.log(`total links: ${links.length}`)

/* oldest to newest converter */
for (let i = links.length-1; i >= 0; i--) {
  console.log(i)
  dumDum.innerHTML += `${links[i]} <br>`
}

```
