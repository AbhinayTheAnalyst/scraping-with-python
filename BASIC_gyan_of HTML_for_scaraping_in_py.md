🔍 1. HTML Structure Ka Basic Gyaan
HTML ek markup language hai, jisme content different tags ke andar hota hai. Har tag ka apna purpose hota hai.

🏷️ 2. Common HTML Tags (Jo tumhein Web Scraping mein kaam aayenge)
Tag	Kaam	Example
<h1> to <h6>	Headings (h1 sabse bada, h6 sabse chhota)	<h1>Main Heading</h1>
<p>	Paragraph (text)	<p>This is a paragraph.</p>
<a>	Anchor tag (link hota hai)	<a href="link.com">Click Here</a>
<img>	Image	<img src="img.jpg" alt="image">
<div>	Division/Container (layout ke liye)	<div class="box">content</div>
<span>	Inline element, mostly styling ke liye	<span style="color:red">Red Text</span>
<ul> / <li>	List banane ke liye	<ul><li>Item 1</li><li>Item 2</li></ul>
<button>	Button	<button>Click</button>

🔑 3. Attributes: id, class, href, src etc.
HTML tags ke andar kuch extra info hoti hai jisse CSS ya JS ya scraping ke time use kiya jaata hai.

💡 Common Attributes:
Attribute	Kaam	Example
id	Unique identity of element	<div id="main-box">content</div>
class	Grouping elements together	<p class="description">text</p>
href	Link ka URL (anchor tag mein)	<a href="link.com">Click</a>
src	Image ya file ka link	<img src="img.png">
alt	Image ka alternate text	<img alt="logo">
title	Tooltip deta hai	<p title="info">Hover me</p>

📌 4. BeautifulSoup mein kaise Use Kare?
✅ Find by tag:
python
Copy code
soup.find("p")
soup.find_all("a")
✅ Find by class:
python
Copy code
soup.find("div", class_="container")
✅ Find by id:
python
Copy code
soup.find("h1", id="main-title")
✅ Get text:
python
Copy code
element.get_text()
✅ Get attributes like href, src:
python
Copy code
link = soup.find("a")
print(link["href"])

image = soup.find("img")
print(image["src"])
🧠 Memory Tip: Human-style
Tum ise is tarah yaad karo:

🧠 "Har HTML element ek dabba hai jisme kuch content ya link ya image hoti hai. Har dabbe (tag) pe ya to naam likha hota hai (id), ya sticker laga hota hai (class), aur usme kuch maal (text, link, image) hota hai."

