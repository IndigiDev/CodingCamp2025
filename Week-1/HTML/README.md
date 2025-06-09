<h1 class="code-line" data-line-start=0 data-line-end=1 ><a id="Lesson_1_HTML_0"></a>Lesson 1: HTML</h1>
<h2 class="code-line" data-line-start=1 data-line-end=2 ><a id="_HyperText_Markup_Language__1"></a><em>HyperText Markup Language</em></h2>
<p class="has-line-data" data-line-start="4" data-line-end="5">HTML defines the structure and content of webpages. It is the frame of the website and one of the fundamental building blocks for all websites. Just about every webpage you see on the internet is made up of the HTML elements you will learn in this lesson.</p>
<h2 class="code-line" data-line-start=6 data-line-end=7 ><a id="HTML_Elements_and_Tags_6"></a>HTML Elements and Tags</h2>
<p class="has-line-data" data-line-start="8" data-line-end="9">In General, an HTML Element is build of three parts:</p>
<ul>
<li class="has-line-data" data-line-start="9" data-line-end="10">The opening HTML Tag</li>
<li class="has-line-data" data-line-start="10" data-line-end="11">The content of the html element</li>
<li class="has-line-data" data-line-start="11" data-line-end="13">The closing HTML Tag</li>
</ul>
<p class="has-line-data" data-line-start="13" data-line-end="15"><strong>The opening tag</strong>:<br>
The opening tag identifies where the HTML element will begin on the page and are made up of angle brackets <code>&lt;&gt;</code> and the HTML element tag name. For example, to create a paragraph tag, you would write <code>&lt;p&gt;</code> to indicate the start of the paragraph.</p>
<p class="has-line-data" data-line-start="16" data-line-end="18"><strong>Closing tag</strong>:<br>
The closing tag identifies where the HTML element ends. It is very similar to the opening tag and is made up of angle brackets <code>&lt;&gt;</code> and the HTML element tag name which should match the opening tag name. What differentiates the end tag is an included forward slash <code>/</code> that is placed in front of the HTML element tag name. For example, to close the paragraph tag we would use <code>&lt;/p&gt;</code>.</p>
<p class="has-line-data" data-line-start="19" data-line-end="21"><strong>The content</strong>:<br>
The content of the HTML will be any content/text placed between the opening and closing tags. For example, to complete the paragraph tag, you would write something like this:</p>
<pre><code class="has-line-data" data-line-start="23" data-line-end="25" class="language-sh">&lt;p&gt;Hello! This is a paragraph element&lt;/p&gt;.
</code></pre>
<p class="has-line-data" data-line-start="26" data-line-end="27">HTML elements are essentially containers for content. There are many HTML Elements that are defined and will be rendered by the browser and we will learn a few that will help us build our first webpage at the end of the lesson. To view the full list of HTML elements, you can view them <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements">here</a></p>
<h3 class="code-line" data-line-start=28 data-line-end=29 ><a id="Void_Elements_28"></a>Void Elements</h3>
<p class="has-line-data" data-line-start="29" data-line-end="30">While we identified the loyout of HTML elements above, there are a few elements that don’t follow the structure we layed out above. These elements are called Void Elements and are named that because they do not wrap around content and are just an opening tag. One example is the image tag <code>&lt;img&gt;</code>, which is used to embed images into a website. This element does not wrap any content and uses a path or link to embed the image. We will go over this more later in the lesson.</p>
<h2 class="code-line" data-line-start=31 data-line-end=32 ><a id="HTML_File_Boilerplate_31"></a>HTML File Boilerplate</h2>
<p class="has-line-data" data-line-start="33" data-line-end="34">HTML files contain the HTMl markup and are used by the browser to display the webpage in the browser. In order for the browser to understand and render the html file, there are a few things that need to be present in the file.</p>
<ol>
<li class="has-line-data" data-line-start="35" data-line-end="36">The file must end in <code>.html</code>. Generally, you would also want the file to be name <code>index.html</code> but this is not a requirement. The <code>index.html</code> is just an easier way for the web server to render the file and is the default file that is expected in a web server directory.</li>
<li class="has-line-data" data-line-start="36" data-line-end="37">The <code>&lt;!DOCTYPE html&gt;</code> element needs to be included and should be the first element in the file. This element identifies the version of html that needs to be used to render the file - just leave it as <code>&lt;!DOCTYPE html&gt;</code> as we won’t really be using any old html versions.</li>
<li class="has-line-data" data-line-start="37" data-line-end="39">The next element that should be on the page is the <code>&lt;html lang='en'&gt;&lt;/html&gt;</code> element which is the root element of the html file and should wrap all other html elements in the page. This should be included in every html file. Notice that we also included the <code>lang</code> attribute in the open tag which indicates that the page is in the english language which assists screen readers to identify how to read the page.
<ul>
<li class="has-line-data" data-line-start="38" data-line-end="39">Html attributes provide additional information about HTML elements and are added in the open tag.</li>
</ul>
</li>
<li class="has-line-data" data-line-start="39" data-line-end="40">The next element that should be included is the <code>&lt;head&gt;&lt;/head&gt;</code> element. This element contains metadata for the website which helps the browser correctly render the html file. You <strong>should not</strong> include any HTML elements that are used to display content on the webpage. Examples of elements that should be included in the head tags are <code>&lt;meta&gt;</code> and <code>&lt;title&gt;&lt;/title&gt;</code> elements. The meta element will be used to identify the encoding charset and the title element is used to set the title of the page that will be displayed in the browser tab and browser’s title bar.</li>
<li class="has-line-data" data-line-start="40" data-line-end="42">The next element is the <code>&lt;body&gt;&lt;/body&gt;</code> element. This is where html elements that display content will be added.</li>
</ol>
<p class="has-line-data" data-line-start="42" data-line-end="43">The following code block shows the complete html boilerplate along with a header tag that displays Hello World! in the browser.</p>
<pre><code class="has-line-data" data-line-start="45" data-line-end="56" class="language-sh">    &lt;!DOCTYPE html&gt;
    &lt;html lang=<span class="hljs-string">"en"</span>&gt;
        &lt;head&gt;
            &lt;meta charseet=<span class="hljs-string">"UTF-8"</span>&gt;
            &lt;title&gt;My First Webpage&lt;/title&gt;
        &lt;/head&gt;
        &lt;body&gt;
            &lt;h1&gt;Hello World!&lt;/h1&gt;
        &lt;/body&gt;
    &lt;/html&gt;
</code></pre>
<h3 class="code-line" data-line-start=57 data-line-end=58 ><a id="Assignment_57"></a>Assignment</h3>
<p class="has-line-data" data-line-start="58" data-line-end="59">Using the VSCode Web terminal, create an <code>index.html</code></p>
<ul>
<li class="has-line-data" data-line-start="59" data-line-end="60">Press <code>ctrl + shift + C</code> to open a new terminal.</li>
<li class="has-line-data" data-line-start="60" data-line-end="61">In the terminal, type <code>touch index.html</code> to create the index.html in the current directory.</li>
<li class="has-line-data" data-line-start="61" data-line-end="62">Open the file using the VSCode Web file explorer and add the boilerplate to the file.</li>
<li class="has-line-data" data-line-start="62" data-line-end="63">Install the live server extension in VSCode if it has not already been installed.</li>
<li class="has-line-data" data-line-start="63" data-line-end="65">Run live server extension and view the rendered file which should just read <code>Hello World!</code>.</li>
</ul>
<h3 class="code-line" data-line-start=65 data-line-end=66 ><a id="VSCode_Shortcut_65"></a>VSCode Shortcut</h3>
<p class="has-line-data" data-line-start="66" data-line-end="67">VScode provides the ability to auto-generate the html boilerplate when an html file is opened. Delete the previous boilerplate and then use the VSCode shortcut. Type <code>!</code> and press enter to use the shortcut. You will notice an extra line which indicates the viewport metadata for the page which can be ignored and is left for you to investigate if you wish.</p>
<h2 class="code-line" data-line-start=68 data-line-end=69 ><a id="HTML_Elements_68"></a>HTML Elements</h2>
<p class="has-line-data" data-line-start="69" data-line-end="70">Now that we have gone over what html elements are and how they can be used in an html file, we will go over some of the different types of tags that can be used for the project at the end of this lesson.</p>
<p class="has-line-data" data-line-start="71" data-line-end="73">The elements will be organized by how they should be used which is important for your page being semantically correct and to help the search engines better understand your site and improve the sites rank in the search engine.<br>
All of these sectiosn and tags can be found in the <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements">mdn web docs</a></p>
<h3 class="code-line" data-line-start=74 data-line-end=75 ><a id="Document_Metadata_74"></a>Document Metadata</h3>
<p class="has-line-data" data-line-start="75" data-line-end="76">Metadata elements that contain information about the page. Metadata includes page title, styles, scripts and data to help the browser render the page.</p>
<ul>
<li class="has-line-data" data-line-start="77" data-line-end="78"><code>&lt;head&gt;</code> - container for the page metadata. Found at the top of the html document.</li>
<li class="has-line-data" data-line-start="78" data-line-end="79"><code>&lt;link&gt;</code> - specifies the relationship between the page and external resources such as stylesheets.</li>
<li class="has-line-data" data-line-start="79" data-line-end="80"><code>&lt;style&gt;</code> - contains direct style information for the page. This will be used only for the page which included the element.</li>
<li class="has-line-data" data-line-start="80" data-line-end="82"><code>&lt;title&gt;</code> - the title of the page which will be used by the browser tabs and title bar.</li>
</ul>
<h3 class="code-line" data-line-start=82 data-line-end=83 ><a id="Content_Sectioning_82"></a>Content Sectioning</h3>
<p class="has-line-data" data-line-start="83" data-line-end="84">Content sectioning elements allow you to organize the html content into logical pieces. These should be used to create a broad outline of your webpage. The following are only a few of the elements for content sectioning.</p>
<ul>
<li class="has-line-data" data-line-start="85" data-line-end="86"><code>&lt;header&gt;</code> - introductory content such as navigation, logos, heading elements, site name, search elements, etc.</li>
<li class="has-line-data" data-line-start="86" data-line-end="87"><code>&lt;h1&gt;, &lt;h2&gt;, ..., &lt;h6&gt;</code> - represent six heading levels. <code>&lt;h1&gt;</code> is the highest and can be used to identify section headings, page titles, etc.</li>
<li class="has-line-data" data-line-start="87" data-line-end="88"><code>&lt;footer&gt;</code> - contains the elements found in the footer for it’s nearest content section. Usually a footer element will be found after the body element and will contain copyright data, author data, footer nav, etc.</li>
<li class="has-line-data" data-line-start="88" data-line-end="90"><code>&lt;main&gt;</code> - main element indicates the dominant content of the page.</li>
</ul>
<h3 class="code-line" data-line-start=90 data-line-end=91 ><a id="Text_Content_90"></a>Text Content</h3>
<p class="has-line-data" data-line-start="91" data-line-end="92">Text content elements are used to organize blocks or sections of content for the page. Contain the content of the page and identify the purpose or are used to structure the content of the page. The following are just a few examples.</p>
<ul>
<li class="has-line-data" data-line-start="93" data-line-end="94"><code>&lt;div&gt;</code> - generic container for content. Has no effect on the content or layout until styled with CSS.</li>
<li class="has-line-data" data-line-start="94" data-line-end="95"><code>&lt;p&gt;</code> - paragraph element which is used to represent blocks of text but are also used to structurally group related content such as images or form fields as well.</li>
<li class="has-line-data" data-line-start="95" data-line-end="96"><code>&lt;ul&gt;</code> - unorder list element which is used to represent a list of items that do not need to be ordered. Usually represented by a bullet point list.</li>
<li class="has-line-data" data-line-start="96" data-line-end="97"><code>&lt;ol&gt;</code> - ordered list element which is used to represent a list of items that should be ordered. Usually represented by a numbered list.</li>
<li class="has-line-data" data-line-start="97" data-line-end="99"><code>&lt;li&gt;</code> - list item that must be used as the content inside either a <code>ul</code> or <code>ol</code> element.</li>
</ul>
<h3 class="code-line" data-line-start=99 data-line-end=100 ><a id="Inline_Text_Semantics_99"></a>Inline Text Semantics</h3>
<p class="has-line-data" data-line-start="100" data-line-end="101">Inline text semantic tags are used to define the meaning, structure, or style a word, line, or any arbitrary piece of text. These elements rendered differently than most of the other elements mentioned because they are rendered inline where the others are rendered as blocks. What this means is that the inline elements be rendered where they are added and not in their own block like every other element.</p>
<ul>
<li class="has-line-data" data-line-start="102" data-line-end="103"><code>&lt;span&gt;</code> - generic inline container which doesn’t inherently represent anything. Used to group elements for styling purposes or because they share attributes. Very similar to a div element with the big difference being that it is rendered inline whereas the div is rendered in its own block.</li>
<li class="has-line-data" data-line-start="103" data-line-end="104"><code>&lt;strong&gt;</code> - used to represent content that has a strong importance on the page. Rendered in bold text by the browser.</li>
<li class="has-line-data" data-line-start="104" data-line-end="105"><code>&lt;em&gt;</code> - used to represent content with emphasis.</li>
<li class="has-line-data" data-line-start="105" data-line-end="106"><code>&lt;a&gt;</code> - the anchor element used to create hyperlinks on the page. The href attribute is required for this element to function properly.</li>
<li class="has-line-data" data-line-start="106" data-line-end="107"><code>&lt;br&gt;</code> - used to create a line break.</li>
<li class="has-line-data" data-line-start="107" data-line-end="109"><code>&lt;u&gt;</code> - used to represent underlined text.</li>
</ul>
<h3 class="code-line" data-line-start=109 data-line-end=110 ><a id="Image_and_Multimedia_109"></a>Image and Multimedia</h3>
<p class="has-line-data" data-line-start="110" data-line-end="111">Multimedia elements for the page</p>
<ul>
<li class="has-line-data" data-line-start="112" data-line-end="113"><code>&lt;img&gt;</code> - image tag that is used to embed images to the page. The <code>src</code> attribute is used to identify the image to embed and can be a url or a path. You should also use both the <code>height</code> and <code>width</code> attributes to set the height and width of the image in the page.</li>
<li class="has-line-data" data-line-start="113" data-line-end="114"><code>&lt;video&gt;</code> - embeds a media player with which supports video playback.</li>
<li class="has-line-data" data-line-start="114" data-line-end="116"><code>&lt;audio&gt;</code> - embeds sound content into the page.</li>
</ul>
<h3 class="code-line" data-line-start=116 data-line-end=117 ><a id="HTML_Attributes_116"></a>HTML Attributes</h3>
<p class="has-line-data" data-line-start="117" data-line-end="118">HTML attributes add additional information about the element. Most commonly used attributes are <code>style</code> for including inline styles on an element, <code>id</code> for adding an identifier for the element (which must be unique on the page), <code>class</code> for adding a grouping identifier for grouping elements for styling or for similar elements on the page, <code>href</code> for creating hyperlinks, <code>src</code> for identifying the src for image or multimedia elements.</p>
<p class="has-line-data" data-line-start="119" data-line-end="120">The following is an example of using attributes for an image element:</p>
<pre><code class="has-line-data" data-line-start="121" data-line-end="123" class="language-sh">&lt;img src=<span class="hljs-string">"https://unsplash.com/photos/big-ben-stands-tall-against-a-cloudy-sky-2qkoVfCUN20"</span> height=<span class="hljs-string">"300px"</span> width=<span class="hljs-string">"200px"</span> alt=<span class="hljs-string">"stylized image of big ben"</span>&gt;
</code></pre>
<p class="has-line-data" data-line-start="124" data-line-end="125">The attributes are used to embed the image found at the provided url and limit it to a height of 300px and a width of 200px. Without the height and width, the image would take the size of the source which can be undesired if the image is really big. The alt attribute provides a description incase the image does not load and also provides better accessibility for screen readers.</p>
<h2 class="code-line" data-line-start=126 data-line-end=127 ><a id="Project_126"></a>Project</h2>
<p class="has-line-data" data-line-start="127" data-line-end="128">Now that we have gone over html elements, html tags, creating and html file, and some useful html elements, we will use our new found information to create a simple webpage that will provide information about yourself. The webpage will be slightly ugly and can be cleaned up with CSS when we reach that section of the curriculum.</p>
<h3 class="code-line" data-line-start=129 data-line-end=130 ><a id="Tasks_129"></a>Tasks</h3>
<ol>
<li class="has-line-data" data-line-start="130" data-line-end="131">Create a new folder - use the <code>mkdir &lt;folder name&gt;</code> command and name it whatever you would like.</li>
<li class="has-line-data" data-line-start="131" data-line-end="134">In that new directory, create an <code>index.html</code>.
<ul>
<li class="has-line-data" data-line-start="132" data-line-end="133">You will need to change to your newly created folder before creating the index.html file by using <code>cd &lt;folder name&gt;</code>.</li>
<li class="has-line-data" data-line-start="133" data-line-end="134">Then when in the correct folder, you will use <code>touch index.html</code>.</li>
</ul>
</li>
<li class="has-line-data" data-line-start="134" data-line-end="136">Open the new <code>index.html</code> file in VSCode Web file explorer and create a page that at least meets the requirements outlined below, but can also contain whatever else you would like.</li>
</ol>
<h3 class="code-line" data-line-start=136 data-line-end=137 ><a id="Requirements_136"></a>Requirements</h3>
<ol>
<li class="has-line-data" data-line-start="137" data-line-end="138">The page should use the html boilerplate you learned in this lesson. (Tip - use the VSCode shortcut to make it easier to set up)</li>
<li class="has-line-data" data-line-start="138" data-line-end="139">You should have a title for the page in the form of ‘FirstName Lastname First Webpage’ that will show in the browser tab and title bar</li>
<li class="has-line-data" data-line-start="139" data-line-end="140">You should have an image - can be any image that you would like as long as it is not inappropriate. Sites like <a href="https://unsplash.com/">unsplash</a> and <a href="https://www.pexels.com/">pexels</a> can help you find images that you may wish to use.</li>
<li class="has-line-data" data-line-start="140" data-line-end="141">You should have a heading element that contains your name.</li>
<li class="has-line-data" data-line-start="141" data-line-end="142">You should have a paragraph that provides some information about why you are attending the IndigiDev coding camp.</li>
<li class="has-line-data" data-line-start="142" data-line-end="143">You should have a list of your top 3 favorite food.</li>
<li class="has-line-data" data-line-start="143" data-line-end="144">You should have an unordered list of your favorite movies.</li>
<li class="has-line-data" data-line-start="144" data-line-end="145">Leave an empty section with a heading of “Projects” that we will fill out with other projects that will be developed through the rest of the coding camp.</li>
</ol>