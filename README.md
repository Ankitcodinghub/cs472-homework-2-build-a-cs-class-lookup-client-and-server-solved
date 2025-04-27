# cs472-homework-2-build-a-cs-class-lookup-client-and-server-solved
**TO GET THIS SOLUTION VISIT:** [CS472 Homework 2-Build a CS Class Lookup Client and Server Solved](https://www.ankitcodinghub.com/product/cs472-homework-2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;121128&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS472  Homework 2-Build a CS Class Lookup Client and Server Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Build a CS Class Lookup Client and Server

Directions and info for this assignment

I stubbed out a lot of this code, so you can thank me later :-).

Basically the objective is to create a client and server that exchange information over a made-up protocol that is simple, but mimics a lot of what you would see working with a real network protocol.

The primary objective of this “protocol” is for the client to send a request to the server with a well-formed packet, requesting information about a class. The server responds with this information. If the client does not provide any command line args, the default is for the client to request information about CS472. The client can also pick another class via the -c option. where an alternative class can be requested. For example -c cs577.

The server also has another trick up its sleeve, it can act as a ping server. This is very useful in real life to support something called health-checks. We will discuss this later in class. For now, the only other thing to understand is that the client can pass an argument [-p “Any message you want”] and the server will echo this message back to the client.

(75% – Programming Component) What to do and hand in

What to hand in? Of course your source code and any specific build instructions. Also include some sample output in a readme file, like im doing here (see below)

The protocol and header

Please understand the protocol defined in cs472-proto.h. This file contains a number of constants and describes the protocol structure in detail. Note that the header has a placeholder for a CMD option. This will indicate if the client is requesting a course lookup or a response to a ping.

The Client

The client application opens up a socket that connects to the server. I hard coded the server address at 127.0.0.1 or localhost. You can change this if you want. Make sure you understand the stubbed out client code well. The client accepts 2 command line parameters. Basically a [-p “ANY

MESSAGE YOU WANT”] parameter to indicate that you want to ping the server and have it echo the request, or a [-c COURSE_ID] parameter to indicate you want the server to look up the course and provide information back.

The Server

The server responds to requests from the client. It binds on 0.0.0.0 – aka all local interfaces. This should work well if you are running locally, you might have to adjust to run on tux. The header cs472-proto.h defines a default port number – 1080. This again might require modification on tux, but should work fine locally.

The server runs in a loop processing client requests. If a request for a class lookup is sent, the server responds with a string about that class. If a ping request is made, the server echos what was sent in the response.

Sample Output

The following is some sample output from my implementation. You don’t need to mirror it exactly, it just shows you what you should be displaying, and how things should be handled.

“` âžœ hw2-echo ./client -p “Hello there server, how are you?” HEADER VALUES Proto Type: PROTO_CS_FUN Proto Ver: VERSION_1 Command: CMD_PING_PONG Direction: DIR_RECV Term: TERM_FALL Course: NONE Pkt Len: 29

RECV FROM SERVER -&gt; PONG: Hello there serv âžœ hw2-echo ./client

HEADER VALUES Proto Type: PROTO_CS_FUN Proto Ver: VERSION_1 Command: CMD_CLASS_INFO Direction: DIR_RECV Term:

TERM_FALL Course: CS472 Pkt Len: 12

RECV FROM SERVER -&gt; CS472: Welcome to computer networks âžœ hw2-echo ./client -c cs577 HEADER VALUES Proto Type:

PROTO_CS_FUN Proto Ver: VERSION_1 Command: CMD_CLASS_INFO Direction: DIR_RECV Term: TERM_FALL Course: cs577 Pkt Len: 12

RECV FROM SERVER -&gt; CS577: Software architecture is important âžœ hw2-echo ./client -c bad

HEADER VALUES Proto Type: PROTO_CS_FUN Proto Ver: VERSION_1 Command: CMD_CLASS_INFO Direction: DIR_RECV Term:

TERM_FALL Course: bad Pkt Len: 12

RECV FROM SERVER -&gt; Requested Course Not Found “`

(25% Question Component) Written Assignment Questions

The programming component of this assignment is worth 75% of your grade. The written component is worth 25%. When you hand in your source code, please provide a pdf or word document that addresses the following:

I am not sure how many of you have even herd of Vint Cerf. Vint is a touring award winner, and is the co-inventor of both TCP,TCP/IP, ARPANET, and is generally considered the father of the Internet. Vint is a gift to our industry, still very active at almost 80 years old. I had the opportunity to sit down with him in a 1:1 meeting to help give him background for a conference I organized where he was a featured keynote, and it was certainly a highlight of my career.

After watching this video, please do a short writeup addressing the following prompts:

1. If you had the opportunity to ask Vint one thing what would that be?

2. What is one thing of interest you took away from this video?
