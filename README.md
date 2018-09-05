# sanlex-vue
Displays for Cologne Sanskrit Lexicon, using vue.js 

Available as web displays at:

>  https://funderburkjim.github.io/sanlex-vue/index.html


### Purpose
This repository aims to scratch two current itches:
* Use a modern Javascript Framework to access the dictionaries at
  the [Cologne Sanskrit Lexicon](sanskrit-lexicon.uni-koeln.de).  
  * The javascript framework chosen is <a href="https://vuejs.org/v2/guide/">Vue 2 </a>.  I've tried learning enough of the React and Angular2 frameworks to 
  do the same , but never got them working. Maybe other programmers with
  familiarity with other frameworks can translate these Vue examples.
  * The access to Cologne data is via a call to its 'apidev' framework. The
   current work in this repository will suggest improvements to that api. 
* Help me improve my Sanskrit vocabulary.  The Basicv0.3 application provides
  a simple way to gain access to the dictionaries using specialized word lists.
  * In my case, I am reading Hitopadesha, and the wordlists will contain the
    words in that text, in order of the text.  This should make it more
    efficient to use the dictionary in conjunction with reading that 
    particular text.
  * This Basicv0.3 application can be easily specialized to other learning
    goals. By forking this repository, and changing the [wordlist](https://github.com/funderburkjim/sanlex-vue/blob/gh-pages/basicv0.3/app-wordlists.js), other
    non-programmers could create useful material for a variety of Sanskrit
    class materials.

### Note on HTTPS and HTTP
The Cologne web site is currently HTTP, and does not support HTTPS.
When making a javascript api call to the Cologne server from an HTTPS web site such as
this one on GitHub, sometimes the connection will be blocked by a security
feature.
As a way to get around this, I made a small application on an HTTPS web site  at https://www.pythonanywhere.com/; all this application does is pass along
information to the Cologne site.  

One current drawback is that the first call to pythonanywhere site sometimes
times out, as my web-site has to, it seems, 'wake up'.  If this happens
to you in running Basicv0.3, etc., just repeat your call.  

If enough people use adaptations of this code and have similar problems,
I'll work on finding a more robust solution.

