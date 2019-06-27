# XML style in DDI (cross-version) 
related issue: TC-162 https://ddi-alliance.atlassian.net/browse/TC-162

# GOAL:
The goal is to have a standard set of style rules for XML schema to be used across versions when possible. Exceptions could still be made but should be documented as a varience from the general rules.

# BACKGROUND:
As we move from hand-crafted to automated production of XML schema we have the opportunity to address issues regarding the style and production rules of the XML used in DDI XML schemas. The issue was originally raised in the context of DDI4 and the need to have clear rules to support the generation of output in multiple bindings. In addition, the rules we currently work under reflect decisions made when we were generally handcrafting XML instances using XML or text editors rather than DDI specific tools. A number of decisions were made to facilitate the ease of creation by reducing entry content (use of attributes rather than elements in many cases). 

Clear rules for the generation of XML schemas from the COGS storage and UML are the minimum. Tools that can handle multiple encodings of the model (e.g. XML and RDF) should not have to have special cases rules built in (like the "foo" property is always an attribute).

A secondary consideration is whether parsing is simpler if just elements (a parser doesn't have to deal with both elements and attributes.)

# SPECIFIC ISSUES:
Should attributes and elements be used or just elements?
* If both are used what is the appropriate balance between their use?
* Is verbosity a valid reason for the attributes?
* If attributes are used how should they be limited?
  * use of xml:lang attribute
* Backwards compatibility issues:
  * CodeValue/ExternalContolledVocabularyEntry
  * International String or Structured International String
  * Attributes associated with identification
  
# CONTRIBUTING TO THE DISCUSSION
To contribute to the discussion please file an issue at https://github.com/ddialliance/DDI-TC-162-Discussion/issues
