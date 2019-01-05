# QuickHelp's Talking Website

This application installs the Talking Website Widget on your Wordpress blog/website.

************
Introduction

Talking Website is a free AI powered Widget that rapidly installs a chatbot on your website. It also has premium features that promise much more!

***********

Requirement

To install the QuickHelp's Talking Website Widget successfully, you'll need to :

1. create an account at https://widget.quickhelp.com.ng/dashboard/signup.php to obtain a chatbot ID.
2. Embed the code generated on your dashboard within the body tag of your website's landing page (or any other page).
3. Engage the dashboard to train your chatbot.
4. For Wordpress sites, download the Talking Website Wordpress widget and install.


********************
Why Talking Website?

With Talking Website, The FAQ is now history as the widget simply enables your website converse with your website visitors, providing the right instant responses, and taking note of their concerns.

Talking Website's backend script, Knowledge Script (QKnows) a is so simple that anyone can immediately create a very smart chatbot in seconds.

By adopting cutting edge natural language processing techniques, Talking Website presently supports text responses, call to actions, audio responses, speech recognition, gesture controls (premium feature), sentiment and entity analysis (premium feature).

Moreover, with 'Quick-E', the custom TW virtual agent, you needn't provide bulky training data-sets to enrich your Conversation User Interface (CUI) as she simply reads your website, and learns from your content on the go in addition to dashboard training! (premium feature)

When On the virtual assistant mode, the Widget is developed to 'take care of business' in your absence, scans for business opportunities, feeds you with relevant news, helps suggest your next move, and even makes some 'digital marketing' efforts for you!(premium feature).

The Talking Website Widget also introduces all the capabilities of the QuickHelp services (please visit www.quickhelp.com.ng) on you website, turning your website into a powerful community service hub thereby gaining more visitors and leads for your business.

With these capabilities, you also become eligible for all QuickHelp's Partnership Schemes (i.e QuickCredit, QuickTaxi etc) thereby opening an additional channels of revenue.

For more information, concerns or suggestions, send an email to support@quickhelp.com.ng

*********************



<p><strong>QuickHelp Knowledge Script (QKnows 0.2,BETA)</strong></p>
<p>The QuickHelp Natural Language Processing (NLP) system is created to be quite simple and fast to develop by the introduction of the QuickHelp&rsquo;s 

Knowledge Script (QKnows). The QKnows is made up of Knowledge Entities (Knowets), scripted data sets engaged to &lsquo;train&rsquo; the chatbot created on 

the QuickHelps Talking Website Dashboard (Please learn more about Talking Website here: https://github.com/SYLMultimedia/quickhelp_TW)</p>
<p>Knowets are made up of Requests, Responses, Flows, Buttons, Gestures, Images, Moods and Actions.</p>
<p>The QKnows algorithm allows users&rsquo; requests to be understood by matching them with the most suitable Knowets. The matching does not need to be 

verbatim or follow any particular order.</p>
<p>When the knowet does not exist or the pre-configured sensitivity is too low, the chatbot returns a negative narrative like &ldquo;Sorry, I do not 

understand you&rdquo;.</p>
<p>The Chatbots sensitivity feature may be configured on the dashboard for premium users.</p>
<p><strong>Structure/Syntax of Qknows</strong></p>
<p>The QuickHelp Knowledge Script (Qknows) is written with Knowledge Entities (Knowets). The script can be written manually, uploaded or simply generated 

with the dashboard. Also, the QuickHelp&rsquo;s Website Reader (QWR) reads to Qknows files which may easily be transferred and reused.</p>
<p><strong>How to Write Knowets</strong></p>
<p>Every knowledge entity (knowet) ends with an '%'.</p>
<p>Knowets are not case sensitive.</p>
<p>Every Knowet is identified and named by its Request. E.g How are you@Great!% is simply named &lsquo;how are you&rsquo; knowet.</p>
<p>Every knowet is started an intent or Request (RQ) and followed by a Response (RS), separated by an '@' e.g.</p>
<p>Knowet: How are you@Fine!% .</p>
<p>The Request is &ldquo;How are you &ldquo;and the Response is &ldquo;Fine!&rdquo;</p>
<p><strong>Flow</strong></p>
<p>A flow is a way of linking one knowet to another to achieve a smoother and seamless conversation.</p>
<p>After the response (RS), introducing ANOTHER single '@' generates what is called a &lsquo;flow&rsquo;.</p>
<p>e.g.</p>
<p>Knowet: Help me@Why?@Thanks%.</p>
<p>The Flow in this example is &lsquo;Thanks&rsquo;.</p>
<p>When the flow is set, the Qknows automatically fires another request. In the example above, the bot responds with a 'why'&nbsp; and flows into 

another&nbsp; Knowledge entity (knowet), seeking the appropriate response for the word "Thanks", if the knowet &lsquo;thanks&rsquo; exists.</p>
<p><strong>Example</strong></p>
<p>Knowet 1: Help me@You need help?@I need help%<br /> Knowet2: I need help@What kind of help do you need?%</p>
<p>&nbsp;</p>
<p><strong>Story</strong></p>
<p>A Qknows Story is a collection of Knowets linked together by flows. Stories are great for sustained or continuous responses to requests. For example, you 

can use a story to explain a concept using multiple Knowets.</p>
<p>Example</p>
<p>Knowet 1: Help me@You need help?@I need help%<br /> Knowet2: created for that purpose@I was created exactly for that purpose.%<br /> Knowet3: I need 

help@What kind of help do you need?@created for that purpose%<br /> </p>
<p>RQ: Help me<br /> RS: You need help?<br /> RS: What kind of help do you need?<br /> RS: I was created exactly for that purpose.</p>
<p>Explanations: Note that the chatbot has a flow from one knowet to another by throwing the next flow and finding the next corresponding knowet. Note also 

that the knowets do not have to follow any particular order.</p>
<p>&nbsp;</p>
<p><strong>Multiple responses</strong></p>
<p>Knowets may also be written to give multiple successive responses. Multiple responses are handled by using the '#' in between responses (RS) e.g How are 

you @Fine#Thank you!%&nbsp;</p>
<p>If you desire, you may also introduce a flow after multiple responses. e.g How are you@Fine#Thank you@your age%. Note that the 'your age' knowet must have 

been created for the flow to work.</p>
<p>&nbsp;</p>
<p><strong>Varying responses</strong></p>
<p>Varying responses make your Chatbots less stupid .ie. smarter. When asked the same question repeatedly, the chatbot simply offer a different answer based 

on the intent or request.</p>
<p>NB: By default, the chatbot detects repetition and will not respond. This can be disabled on the dashboard is not desired if you are on Premium plan.<br 

/> The Qknow script allows you to have varying responses for a simple request. This is achieved by introducing the &lsquo;|&rsquo; between the knowledge 

element.</p>
<p>Example</p>
<p>Where are you?@I am in Lagos | I am not around. %</p>
<p>This example suggests 2 variations of responses i.e &rsquo;I am in Lagos&rsquo; or &lsquo;I am not around&rsquo;, randomly. <br /> NB: This feature is 

only available to premium users.</p>
<p><strong>Sentiments Detection</strong></p>
<p>The QKnows is enabled to identify the sentiment of requests. When it detects a high or low sentiment, it looks for a matching Knowet, makes the 

appropriate response but also throws a high or low sentiment response, via a flow. &nbsp;Therefore the high and low sentiment knowets must also be pre-

defined.</p>
<p>Example</p>
<p>Knowet1:What an idiot you are@Wao#Idiot is a strong word!%<br /> Knowet2:low_knows@now you are making me very sad.% (predefined on dashboard)<br /> RQ: 

What an idiot you are!<br /> RS: Wao, Idiot is a strong word!<br /> RS: Now, you are making me very sad.<br /> Explanation: Qknows picks the sentiment of the 

request as low, and adds a &lsquo;low knows&rsquo; flow, automatically. This also happens when it detects a happy or high spirited request like &ldquo;You 

are smart!&rdquo;.</p>
<p>&nbsp;</p>
<p><strong>Moods</strong></p>
<p>Moods are ways of suggesting how your chatbot should respond per knowet. By default, the QKnows is made up of 3 mood templates: Low, Normal and High.</p>
<p>Premium users will be able to configure more variants.</p>
<p>When the mood is not specified, the chatbot defaults to Normal. The High mood is reflected with a highlighted text response. For now, the low mood is 

reflected by a coloured text response, like red, orange or brown.</p>
<p>Example</p>
<p>How are you@Fine#Thank you@@@mood:high %</p>
<p>This knowet example will expect a &lsquo;How are you&rsquo; request to return &lsquo;Fine&rsquo;, &rsquo;Thank you&rsquo; in successive responses, with 

Highlighted texts, suggesting a great mood.</p>
<p>Images, links, gestures are also handled similarly (Please see the Knowet reference for more examples)</p>
<p><strong>Complex requests</strong></p>
<p>Complex requests are requests that are made up complex sentences i.e compound sentences that have two or more concepts, but joined together by 

punctuations. e.g &lsquo;I am home. Have you cooked?&rsquo;</p>
<p>Qknows automatically detects complex requests and breaks them down into simple individual requests, treating each component as an individual knowet. For 

now, Qknows does not relate each of the independent responses.</p>
<p>NB: This feature is only functional for premium users.</p>
<p><strong>Contexts</strong></p>
<p>Although this is still anon going development and not yet perfected, Qknows handles context by identifying key entities within the requests. For example, 

a request like &ldquo;Do you have some candy?&rdquo; will automatically triggers the context &lsquo;candy&rsquo;. Further requests like &ldquo;where did you 

buy it?&rdquo; will be reconverted to &ldquo;when did you buy candy&rdquo; before firing the appropriate knowet.</p>
<p>Example 1, for the following given knowet:</p>
<p>Knowet : Help me bring my bag@Ok#Where is it?%<br /> RQ: It is in the bathroom!</p>
<p>Explanation:</p>
<p>The RQ will be reconverted to &ldquo;bag is in the bathroom&rdquo; and that fires the &lsquo;bag is in the bathroom&rdquo; Knowet if it exists.</p>
<p>Example 2, for the following given knowet:</p>
<p>Knowet : I Do you love dancing?@Yes&nbsp; I do%<br /> RQ: What about Swimming?</p>
<p>Knowet : I Do you swim?@Yes&nbsp; I do%</p>
<p>Explanation:</p>
<p>QKnows will identify the entity &lsquo;swimming&rsquo; and the Context trigger &ldquo;what about&rdquo; and the Request will be reconverted to &ldquo;Do 

you love Swimming&rdquo; and that fires the &lsquo;Do you love swimming&rdquo; Knowet if it exists.</p>
<p>Note that Knowet &lsquo;Do you love swimming&rsquo; does not exist but the closest knowet fires &lsquo;Do you swim?&rsquo;.</p>
<p><strong>Say it again</strong></p>
<p>The QKnows allows your chatbot users to make a polite request for repetitions of previous answers. E.g</p>
<p>Knowet: Are you smart @Yes, I am trying%</p>
<p>RQ: Are you smart?<br /> RS: Yes, I am trying.<br /> RQ: What did you say?<br /> RS: I said Yes, I am trying.</p>
<p>Explanation: The QKnows detects the intent &lsquo;what did you say &lsquo;and recognizes it as a request for repetition.</p>
<p><strong>&nbsp;</strong></p>
<p><strong>Agreements, yes/no responses</strong></p>
<p>The Qknows is also able to throw a pre-flow when it detects a yes or no response. It does this by prefixing a yes or no (or synonyms) to original request 

and throwing is as a flow.</p>
<p>Example</p>
<p>Knowet1: What is the meaning of KNOWET@KNOWET &nbsp;means knowledge entity@ &nbsp;just knowing this%<br /> Knowet2: Just knowing this@ Are you just 

knowing this?!%<br /> Knowet3: <strong>Yes</strong> &nbsp;Just knowing this @ Oh!, Ithought you were following me!%</p>
<p><br /> RQ:What is the meaning of KNOWET?<br /> RS: KNOWET &nbsp;means knowledge entity.<br /> RS: Are you just knowing this?!<br /> RQ:Yes<br /> RS:Oh!, 

Ithought you were following me!</p>
<p><strong>Explanations:</strong></p>
<p>Note that Knowet 1 has a flow &lsquo;just knowing this&rsquo;. This flow will search for knowet2 and fire the response &lsquo;Are you just knowing this?!

&rsquo;. If a &lsquo;yes&rsquo; is returned, Knowet3 is triggered if it exists. If not, it will default back to Knowet 2.</p>
<p>Caution:&nbsp; This might create an unwanted loop so all Yes/No (polar) question knowets must always be followed by a corresponding yes or no knowets for 

the appropriate reponses.</p>
<p><strong>&nbsp;</strong></p>
<p><strong>Wikipedia</strong></p>
<p>The QKnows sometimes defaults to Wikipedia for unknown requests thereby creating an undesirable response. &nbsp;<br /> </p>
<p><strong>Knowets 

Reference&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbs

p;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong></p>
<p>RQ@@@how are you?% Creates a request call to action button. e.g How are you@@@Find out here%.<br /> RQ@Great!@@how are you?% Creates a request call to 

action button after a response. e.g How are you@@@Find out here%.<br /> RQ@@@how are you?(link:&rsquo;http://yoururl&rsquo;) % Creates a button. e.g How are 

you@@@Find out here(link:&rsquo;http://yoururl&rsquo;)%.<br /> RQ@Great!@@mood:high % Suggests a response &lsquo;Great&rsquo; with a high mood. <br /> 

RQ@Bad@@ mood:low % suggests a response &lsquo;Bad&rsquo; with a low mood. <br /> RQ@Get lost@@ gesture:dock% Suggests a response &rsquo;Get 

lost&rsquo;&nbsp; with a &nbsp;gesture. In this case, the gesture is docking i.e the AI agent minimizes.<br /> RQ@I am Typing!@@ action:type:Sugar% Suggests 

a response &rsquo;I am typing&rsquo;&nbsp; with an action. In this case, the action is to type the word &lsquo;Sugar&rsquo;.</p>
<p>RQ@This is my face@@ image:&rsquo;imageurl.jpg&rsquo;% Suggests a response &rsquo;This is my face&rsquo; with the image displayed referencing the url 

&lsquo;imageurl.jpg&rsquo;.</p>
<p>&nbsp;</p>
<p><strong>Further Development</strong></p>
<p>The QKnows is a still a very na&iuml;ve or over-simplified attempt at NLP. It is also still adjudged complicated compared to the original dream of having 

a true scripting language for non-technical users. Also, initial testing is proving that the Qknows is still far from being consistent with intended 

responses.</p>
<p>However, the QuickHelp development team has proposed Qknows as it is, while it works on the following:</p>
<ul>
<li>Dynamic Entities</li>
<li>More Context Triggers</li>
<li>Stemming and Lemmalization</li>
<li>Parts of Speech Tagging</li>
<li>Shallow Parsing</li>
<li>Constituency and Dependency Parsing</li>
<li>Emoticons and shorthand</li>
<li>Summarization</li>
</ul>
<p>Remember that to use Qknows, you need to sign up for QuickHelp's TalkingWebsite here: https://widget.quickhelp.com.ng/dashboard/signup.php</p>
<p>For Suggestions, criticism, feedbacks or contributions, please send an email to Tosin at <a 

href="mailto:qknows@quickhelp.com.ng">qknows@quickhelp.com.ng</a></p>
<p>&nbsp;</p>
<p>Development Team<br /> <br /> Oluwatosin Odubela<br /> Lead Programmer<br /> <br /> Akin Akinseinde<br /> Data Scientist<br /> <br /> Olayinka odubela<br 

/> Linguistics <br /> </p>
<p>Qknows Copyright 2019. All rights reserved.</p>

