# api documentation for  [xmlbuilder (v8.2.2)](http://github.com/oozcitak/xmlbuilder-js)  [![npm package](https://img.shields.io/npm/v/npmdoc-xmlbuilder.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-xmlbuilder) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-xmlbuilder.svg)](https://travis-ci.org/npmdoc/node-npmdoc-xmlbuilder)
#### An XML builder for node.js

[![NPM](https://nodei.co/npm/xmlbuilder.png?downloads=true)](https://www.npmjs.com/package/xmlbuilder)

[![apidoc](https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-xmlbuilder_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Ozgur Ozcitak",
        "email": "oozcitak@gmail.com"
    },
    "bugs": {
        "url": "http://github.com/oozcitak/xmlbuilder-js/issues"
    },
    "contributors": [],
    "dependencies": {},
    "description": "An XML builder for node.js",
    "devDependencies": {
        "coffee-coverage": "*",
        "coffee-script": "*",
        "coveralls": "*",
        "istanbul": "*",
        "mocha": "*"
    },
    "directories": {},
    "dist": {
        "shasum": "69248673410b4ba42e1a6136551d2922335aa773",
        "tarball": "https://registry.npmjs.org/xmlbuilder/-/xmlbuilder-8.2.2.tgz"
    },
    "engines": {
        "node": ">=4.0"
    },
    "gitHead": "ab5987b12bc06e4da8c37cd7fec8f93085d96d28",
    "homepage": "http://github.com/oozcitak/xmlbuilder-js",
    "keywords": [
        "xml",
        "xmlbuilder"
    ],
    "license": "MIT",
    "main": "./lib/index",
    "maintainers": [
        {
            "name": "oozcitak",
            "email": "oozcitak@gmail.com"
        }
    ],
    "name": "xmlbuilder",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/oozcitak/xmlbuilder-js.git"
    },
    "scripts": {
        "postpublish": "rm -rf lib",
        "prepublish": "coffee -co lib src",
        "test": "mocha && istanbul report text lcov"
    },
    "version": "8.2.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module xmlbuilder](#apidoc.module.xmlbuilder)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLAttribute (parent, name, value)](#apidoc.element.xmlbuilder.XMLAttribute)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLCData (parent, text)](#apidoc.element.xmlbuilder.XMLCData)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLComment (parent, text)](#apidoc.element.xmlbuilder.XMLComment)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDAttList (parent, elementName, attributeName, attributeType, defaultValueType, defaultValue)](#apidoc.element.xmlbuilder.XMLDTDAttList)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDElement (parent, name, value)](#apidoc.element.xmlbuilder.XMLDTDElement)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDEntity (parent, pe, name, value)](#apidoc.element.xmlbuilder.XMLDTDEntity)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDNotation (parent, name, value)](#apidoc.element.xmlbuilder.XMLDTDNotation)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDeclaration (parent, version, encoding, standalone)](#apidoc.element.xmlbuilder.XMLDeclaration)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocType (parent, pubID, sysID)](#apidoc.element.xmlbuilder.XMLDocType)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocument (options)](#apidoc.element.xmlbuilder.XMLDocument)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocumentCB (options, onData, onEnd)](#apidoc.element.xmlbuilder.XMLDocumentCB)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLElement (parent, name, attributes)](#apidoc.element.xmlbuilder.XMLElement)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLNode (parent)](#apidoc.element.xmlbuilder.XMLNode)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLProcessingInstruction (parent, target, value)](#apidoc.element.xmlbuilder.XMLProcessingInstruction)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLRaw (parent, text)](#apidoc.element.xmlbuilder.XMLRaw)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStreamWriter (stream, options)](#apidoc.element.xmlbuilder.XMLStreamWriter)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStringWriter (options)](#apidoc.element.xmlbuilder.XMLStringWriter)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStringifier (options)](#apidoc.element.xmlbuilder.XMLStringifier)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLText (parent, text)](#apidoc.element.xmlbuilder.XMLText)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLWriterBase (options)](#apidoc.element.xmlbuilder.XMLWriterBase)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>begin (options, onData, onEnd)](#apidoc.element.xmlbuilder.begin)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>create (name, xmldec, doctype, options)](#apidoc.element.xmlbuilder.create)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>streamWriter (stream, options)](#apidoc.element.xmlbuilder.streamWriter)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>stringWriter (options)](#apidoc.element.xmlbuilder.stringWriter)
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>Utility
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLAttribute.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLCData.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLComment.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDAttList.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDElement.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDEntity.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDNotation.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDeclaration.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocType.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocument.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocumentCB.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLElement.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLNode.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLProcessingInstruction.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLRaw.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStreamWriter.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStringWriter.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStringifier.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLText.prototype
1.  object <span class="apidocSignatureSpan">xmlbuilder.</span>XMLWriterBase.prototype

#### [module xmlbuilder.Utility](#apidoc.module.xmlbuilder.Utility)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>assign ()](#apidoc.element.xmlbuilder.Utility.assign)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>camelCase (val)](#apidoc.element.xmlbuilder.Utility.camelCase)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>capitalize (val)](#apidoc.element.xmlbuilder.Utility.capitalize)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>isArray (val)](#apidoc.element.xmlbuilder.Utility.isArray)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>isEmpty (val)](#apidoc.element.xmlbuilder.Utility.isEmpty)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>isFunction (val)](#apidoc.element.xmlbuilder.Utility.isFunction)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>isObject (val)](#apidoc.element.xmlbuilder.Utility.isObject)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>isPlainObject (val)](#apidoc.element.xmlbuilder.Utility.isPlainObject)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>kebabCase (val)](#apidoc.element.xmlbuilder.Utility.kebabCase)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>snakeCase (val)](#apidoc.element.xmlbuilder.Utility.snakeCase)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>titleCase (val)](#apidoc.element.xmlbuilder.Utility.titleCase)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>words (val)](#apidoc.element.xmlbuilder.Utility.words)

#### [module xmlbuilder.XMLAttribute](#apidoc.module.xmlbuilder.XMLAttribute)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLAttribute (parent, name, value)](#apidoc.element.xmlbuilder.XMLAttribute.XMLAttribute)

#### [module xmlbuilder.XMLAttribute.prototype](#apidoc.module.xmlbuilder.XMLAttribute.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLAttribute.prototype.</span>clone ()](#apidoc.element.xmlbuilder.XMLAttribute.prototype.clone)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLAttribute.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLAttribute.prototype.toString)

#### [module xmlbuilder.XMLCData](#apidoc.module.xmlbuilder.XMLCData)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLCData (parent, text)](#apidoc.element.xmlbuilder.XMLCData.XMLCData)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLCData.</span>__super__

#### [module xmlbuilder.XMLCData.prototype](#apidoc.module.xmlbuilder.XMLCData.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLCData.prototype.</span>clone ()](#apidoc.element.xmlbuilder.XMLCData.prototype.clone)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLCData.prototype.</span>constructor (parent, text)](#apidoc.element.xmlbuilder.XMLCData.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLCData.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLCData.prototype.toString)

#### [module xmlbuilder.XMLComment](#apidoc.module.xmlbuilder.XMLComment)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLComment (parent, text)](#apidoc.element.xmlbuilder.XMLComment.XMLComment)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLComment.</span>__super__

#### [module xmlbuilder.XMLComment.prototype](#apidoc.module.xmlbuilder.XMLComment.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLComment.prototype.</span>clone ()](#apidoc.element.xmlbuilder.XMLComment.prototype.clone)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLComment.prototype.</span>constructor (parent, text)](#apidoc.element.xmlbuilder.XMLComment.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLComment.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLComment.prototype.toString)

#### [module xmlbuilder.XMLDTDAttList](#apidoc.module.xmlbuilder.XMLDTDAttList)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDAttList (parent, elementName, attributeName, attributeType, defaultValueType, defaultValue)](#apidoc.element.xmlbuilder.XMLDTDAttList.XMLDTDAttList)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLDTDAttList.</span>__super__

#### [module xmlbuilder.XMLDTDAttList.prototype](#apidoc.module.xmlbuilder.XMLDTDAttList.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDAttList.prototype.</span>constructor (parent, elementName, attributeName, attributeType, defaultValueType, defaultValue)](#apidoc.element.xmlbuilder.XMLDTDAttList.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDAttList.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLDTDAttList.prototype.toString)

#### [module xmlbuilder.XMLDTDElement](#apidoc.module.xmlbuilder.XMLDTDElement)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDElement (parent, name, value)](#apidoc.element.xmlbuilder.XMLDTDElement.XMLDTDElement)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLDTDElement.</span>__super__

#### [module xmlbuilder.XMLDTDElement.prototype](#apidoc.module.xmlbuilder.XMLDTDElement.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDElement.prototype.</span>constructor (parent, name, value)](#apidoc.element.xmlbuilder.XMLDTDElement.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDElement.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLDTDElement.prototype.toString)

#### [module xmlbuilder.XMLDTDEntity](#apidoc.module.xmlbuilder.XMLDTDEntity)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDEntity (parent, pe, name, value)](#apidoc.element.xmlbuilder.XMLDTDEntity.XMLDTDEntity)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLDTDEntity.</span>__super__

#### [module xmlbuilder.XMLDTDEntity.prototype](#apidoc.module.xmlbuilder.XMLDTDEntity.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDEntity.prototype.</span>constructor (parent, pe, name, value)](#apidoc.element.xmlbuilder.XMLDTDEntity.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDEntity.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLDTDEntity.prototype.toString)

#### [module xmlbuilder.XMLDTDNotation](#apidoc.module.xmlbuilder.XMLDTDNotation)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDNotation (parent, name, value)](#apidoc.element.xmlbuilder.XMLDTDNotation.XMLDTDNotation)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLDTDNotation.</span>__super__

#### [module xmlbuilder.XMLDTDNotation.prototype](#apidoc.module.xmlbuilder.XMLDTDNotation.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDNotation.prototype.</span>constructor (parent, name, value)](#apidoc.element.xmlbuilder.XMLDTDNotation.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDNotation.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLDTDNotation.prototype.toString)

#### [module xmlbuilder.XMLDeclaration](#apidoc.module.xmlbuilder.XMLDeclaration)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDeclaration (parent, version, encoding, standalone)](#apidoc.element.xmlbuilder.XMLDeclaration.XMLDeclaration)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLDeclaration.</span>__super__

#### [module xmlbuilder.XMLDeclaration.prototype](#apidoc.module.xmlbuilder.XMLDeclaration.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDeclaration.prototype.</span>constructor (parent, version, encoding, standalone)](#apidoc.element.xmlbuilder.XMLDeclaration.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDeclaration.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLDeclaration.prototype.toString)

#### [module xmlbuilder.XMLDocType](#apidoc.module.xmlbuilder.XMLDocType)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocType (parent, pubID, sysID)](#apidoc.element.xmlbuilder.XMLDocType.XMLDocType)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.</span>__super__

#### [module xmlbuilder.XMLDocType.prototype](#apidoc.module.xmlbuilder.XMLDocType.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>att (elementName, attributeName, attributeType, defaultValueType, defaultValue)](#apidoc.element.xmlbuilder.XMLDocType.prototype.att)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>attList (elementName, attributeName, attributeType, defaultValueType, defaultValue)](#apidoc.element.xmlbuilder.XMLDocType.prototype.attList)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>constructor (parent, pubID, sysID)](#apidoc.element.xmlbuilder.XMLDocType.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>ele (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.ele)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>element (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.element)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>ent (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.ent)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>entity (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.entity)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>not (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.not)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>notation (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.notation)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>pEntity (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.pEntity)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>pent (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.pent)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLDocType.prototype.toString)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>up ()](#apidoc.element.xmlbuilder.XMLDocType.prototype.up)

#### [module xmlbuilder.XMLDocument](#apidoc.module.xmlbuilder.XMLDocument)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocument (options)](#apidoc.element.xmlbuilder.XMLDocument.XMLDocument)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLDocument.</span>__super__

#### [module xmlbuilder.XMLDocument.prototype](#apidoc.module.xmlbuilder.XMLDocument.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocument.prototype.</span>constructor (options)](#apidoc.element.xmlbuilder.XMLDocument.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocument.prototype.</span>end (writer)](#apidoc.element.xmlbuilder.XMLDocument.prototype.end)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocument.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLDocument.prototype.toString)

#### [module xmlbuilder.XMLDocumentCB](#apidoc.module.xmlbuilder.XMLDocumentCB)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocumentCB (options, onData, onEnd)](#apidoc.element.xmlbuilder.XMLDocumentCB.XMLDocumentCB)

#### [module xmlbuilder.XMLDocumentCB.prototype](#apidoc.module.xmlbuilder.XMLDocumentCB.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>a ()](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.a)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>att ()](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.att)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>attList (elementName, attributeName, attributeType, defaultValueType, defaultValue)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.attList)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>attribute (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.attribute)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>c (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.c)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>cdata (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.cdata)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>closeNode (node)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.closeNode)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>com (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.com)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>comment (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.comment)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>d (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.d)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>dat (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.dat)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>dec (version, encoding, standalone)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.dec)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>declaration (version, encoding, standalone)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.declaration)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>doctype (root, pubID, sysID)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.doctype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>dtd (root, pubID, sysID)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.dtd)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>dtdElement (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.dtdElement)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>e (name, attributes, text)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.e)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>ele ()](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.ele)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>element (name, attributes, text)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.element)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>end ()](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.end)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>ent (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.ent)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>entity (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.entity)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>i (target, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.i)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>ins (target, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.ins)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>instruction (target, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.instruction)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>n (name, attributes, text)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.n)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>nod (name, attributes, text)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.nod)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>node (name, attributes, text)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.node)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>not (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.not)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>notation (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.notation)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>onData (chunk)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.onData)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>onEnd ()](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.onEnd)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>openCurrent ()](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.openCurrent)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>openNode (node)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.openNode)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>pEntity (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.pEntity)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>pent (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.pent)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>r (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.r)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>raw (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.raw)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>t (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.t)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>text (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.text)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>txt (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.txt)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>up ()](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.up)

#### [module xmlbuilder.XMLElement](#apidoc.module.xmlbuilder.XMLElement)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLElement (parent, name, attributes)](#apidoc.element.xmlbuilder.XMLElement.XMLElement)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLElement.</span>__super__

#### [module xmlbuilder.XMLElement.prototype](#apidoc.module.xmlbuilder.XMLElement.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLElement.prototype.</span>a (name, value)](#apidoc.element.xmlbuilder.XMLElement.prototype.a)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLElement.prototype.</span>att (name, value)](#apidoc.element.xmlbuilder.XMLElement.prototype.att)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLElement.prototype.</span>attribute (name, value)](#apidoc.element.xmlbuilder.XMLElement.prototype.attribute)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLElement.prototype.</span>clone ()](#apidoc.element.xmlbuilder.XMLElement.prototype.clone)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLElement.prototype.</span>constructor (parent, name, attributes)](#apidoc.element.xmlbuilder.XMLElement.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLElement.prototype.</span>removeAttribute (name)](#apidoc.element.xmlbuilder.XMLElement.prototype.removeAttribute)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLElement.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLElement.prototype.toString)

#### [module xmlbuilder.XMLNode](#apidoc.module.xmlbuilder.XMLNode)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLNode (parent)](#apidoc.element.xmlbuilder.XMLNode.XMLNode)

#### [module xmlbuilder.XMLNode.prototype](#apidoc.module.xmlbuilder.XMLNode.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>c (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.c)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>cdata (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.cdata)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>com (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.com)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>comment (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.comment)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>commentAfter (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.commentAfter)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>commentBefore (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.commentBefore)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>d (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.d)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>dat (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.dat)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>dec (version, encoding, standalone)](#apidoc.element.xmlbuilder.XMLNode.prototype.dec)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>declaration (version, encoding, standalone)](#apidoc.element.xmlbuilder.XMLNode.prototype.declaration)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>doc ()](#apidoc.element.xmlbuilder.XMLNode.prototype.doc)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>doctype (pubID, sysID)](#apidoc.element.xmlbuilder.XMLNode.prototype.doctype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>document ()](#apidoc.element.xmlbuilder.XMLNode.prototype.document)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>dtd (pubID, sysID)](#apidoc.element.xmlbuilder.XMLNode.prototype.dtd)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>e (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.e)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>ele (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.ele)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>element (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.element)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>end (options)](#apidoc.element.xmlbuilder.XMLNode.prototype.end)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>i (target, value)](#apidoc.element.xmlbuilder.XMLNode.prototype.i)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>importDocument (doc)](#apidoc.element.xmlbuilder.XMLNode.prototype.importDocument)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>importXMLBuilder (doc)](#apidoc.element.xmlbuilder.XMLNode.prototype.importXMLBuilder)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>ins (target, value)](#apidoc.element.xmlbuilder.XMLNode.prototype.ins)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>insertAfter (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.insertAfter)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>insertBefore (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.insertBefore)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>instruction (target, value)](#apidoc.element.xmlbuilder.XMLNode.prototype.instruction)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>instructionAfter (target, value)](#apidoc.element.xmlbuilder.XMLNode.prototype.instructionAfter)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>instructionBefore (target, value)](#apidoc.element.xmlbuilder.XMLNode.prototype.instructionBefore)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>n (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.n)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>next ()](#apidoc.element.xmlbuilder.XMLNode.prototype.next)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>nod (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.nod)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>node (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.node)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>prev ()](#apidoc.element.xmlbuilder.XMLNode.prototype.prev)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>r (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.r)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>raw (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.raw)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>remove ()](#apidoc.element.xmlbuilder.XMLNode.prototype.remove)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>root ()](#apidoc.element.xmlbuilder.XMLNode.prototype.root)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>t (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.t)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>text (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.text)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>txt (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.txt)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>u ()](#apidoc.element.xmlbuilder.XMLNode.prototype.u)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>up ()](#apidoc.element.xmlbuilder.XMLNode.prototype.up)

#### [module xmlbuilder.XMLProcessingInstruction](#apidoc.module.xmlbuilder.XMLProcessingInstruction)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLProcessingInstruction (parent, target, value)](#apidoc.element.xmlbuilder.XMLProcessingInstruction.XMLProcessingInstruction)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLProcessingInstruction.</span>__super__

#### [module xmlbuilder.XMLProcessingInstruction.prototype](#apidoc.module.xmlbuilder.XMLProcessingInstruction.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLProcessingInstruction.prototype.</span>clone ()](#apidoc.element.xmlbuilder.XMLProcessingInstruction.prototype.clone)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLProcessingInstruction.prototype.</span>constructor (parent, target, value)](#apidoc.element.xmlbuilder.XMLProcessingInstruction.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLProcessingInstruction.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLProcessingInstruction.prototype.toString)

#### [module xmlbuilder.XMLRaw](#apidoc.module.xmlbuilder.XMLRaw)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLRaw (parent, text)](#apidoc.element.xmlbuilder.XMLRaw.XMLRaw)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLRaw.</span>__super__

#### [module xmlbuilder.XMLRaw.prototype](#apidoc.module.xmlbuilder.XMLRaw.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLRaw.prototype.</span>clone ()](#apidoc.element.xmlbuilder.XMLRaw.prototype.clone)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLRaw.prototype.</span>constructor (parent, text)](#apidoc.element.xmlbuilder.XMLRaw.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLRaw.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLRaw.prototype.toString)

#### [module xmlbuilder.XMLStreamWriter](#apidoc.module.xmlbuilder.XMLStreamWriter)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStreamWriter (stream, options)](#apidoc.element.xmlbuilder.XMLStreamWriter.XMLStreamWriter)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.</span>__super__

#### [module xmlbuilder.XMLStreamWriter.prototype](#apidoc.module.xmlbuilder.XMLStreamWriter.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>attribute (att)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.attribute)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>cdata (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.cdata)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>comment (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.comment)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>constructor (stream, options)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>declaration (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.declaration)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>docType (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.docType)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>document (doc)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.document)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>dtdAttList (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.dtdAttList)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>dtdElement (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.dtdElement)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>dtdEntity (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.dtdEntity)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>dtdNotation (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.dtdNotation)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>element (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.element)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>endline (node)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.endline)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>processingInstruction (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.processingInstruction)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>raw (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.raw)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>text (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.text)

#### [module xmlbuilder.XMLStringWriter](#apidoc.module.xmlbuilder.XMLStringWriter)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStringWriter (options)](#apidoc.element.xmlbuilder.XMLStringWriter.XMLStringWriter)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.</span>__super__

#### [module xmlbuilder.XMLStringWriter.prototype](#apidoc.module.xmlbuilder.XMLStringWriter.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>attribute (att)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.attribute)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>cdata (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.cdata)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>closeNode (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.closeNode)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>comment (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.comment)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>constructor (options)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>declaration (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.declaration)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>docType (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.docType)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>document (doc)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.document)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>dtdAttList (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.dtdAttList)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>dtdElement (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.dtdElement)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>dtdEntity (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.dtdEntity)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>dtdNotation (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.dtdNotation)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>element (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.element)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>openNode (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.openNode)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>processingInstruction (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.processingInstruction)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>raw (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.raw)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>text (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.text)

#### [module xmlbuilder.XMLStringifier](#apidoc.module.xmlbuilder.XMLStringifier)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStringifier (options)](#apidoc.element.xmlbuilder.XMLStringifier.XMLStringifier)

#### [module xmlbuilder.XMLStringifier.prototype](#apidoc.module.xmlbuilder.XMLStringifier.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>applyCase (str)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.applyCase)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>assertLegalChar (str)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.assertLegalChar)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>attEscape (str)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.attEscape)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>attName (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.attName)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>attValue (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.attValue)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>cdata (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.cdata)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>comment (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.comment)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>dtdAttDefault (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdAttDefault)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>dtdAttType (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdAttType)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>dtdElementValue (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdElementValue)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>dtdEntityValue (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdEntityValue)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>dtdNData (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdNData)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>dtdPubID (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdPubID)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>dtdSysID (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdSysID)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>elEscape (str)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.elEscape)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>eleName (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.eleName)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>eleText (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.eleText)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>insTarget (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.insTarget)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>insValue (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.insValue)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>raw (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.raw)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>xmlEncoding (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.xmlEncoding)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>xmlStandalone (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.xmlStandalone)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>xmlVersion (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.xmlVersion)
1.  string <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>convertAttKey
1.  string <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>convertCDataKey
1.  string <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>convertCommentKey
1.  string <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>convertPIKey
1.  string <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>convertRawKey
1.  string <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>convertTextKey

#### [module xmlbuilder.XMLText](#apidoc.module.xmlbuilder.XMLText)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLText (parent, text)](#apidoc.element.xmlbuilder.XMLText.XMLText)
1.  object <span class="apidocSignatureSpan">xmlbuilder.XMLText.</span>__super__

#### [module xmlbuilder.XMLText.prototype](#apidoc.module.xmlbuilder.XMLText.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLText.prototype.</span>clone ()](#apidoc.element.xmlbuilder.XMLText.prototype.clone)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLText.prototype.</span>constructor (parent, text)](#apidoc.element.xmlbuilder.XMLText.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLText.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLText.prototype.toString)

#### [module xmlbuilder.XMLWriterBase](#apidoc.module.xmlbuilder.XMLWriterBase)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLWriterBase (options)](#apidoc.element.xmlbuilder.XMLWriterBase.XMLWriterBase)

#### [module xmlbuilder.XMLWriterBase.prototype](#apidoc.module.xmlbuilder.XMLWriterBase.prototype)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLWriterBase.prototype.</span>set (options)](#apidoc.element.xmlbuilder.XMLWriterBase.prototype.set)
1.  [function <span class="apidocSignatureSpan">xmlbuilder.XMLWriterBase.prototype.</span>space (level)](#apidoc.element.xmlbuilder.XMLWriterBase.prototype.space)



# <a name="apidoc.module.xmlbuilder"></a>[module xmlbuilder](#apidoc.module.xmlbuilder)

#### <a name="apidoc.element.xmlbuilder.XMLAttribute"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLAttribute (parent, name, value)](#apidoc.element.xmlbuilder.XMLAttribute)
- description and source-code
```javascript
function XMLAttribute(parent, name, value) {
  this.options = parent.options;
  this.stringify = parent.stringify;
  if (name == null) {
    throw new Error("Missing attribute name of element " + parent.name);
  }
  if (value == null) {
    throw new Error("Missing attribute value for attribute " + name + " of element " + parent.name);
  }
  this.name = this.stringify.attName(name);
  this.value = this.stringify.attValue(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLCData"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLCData (parent, text)](#apidoc.element.xmlbuilder.XMLCData)
- description and source-code
```javascript
function XMLCData(parent, text) {
  XMLCData.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing CDATA text");
  }
  this.text = this.stringify.cdata(text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLComment"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLComment (parent, text)](#apidoc.element.xmlbuilder.XMLComment)
- description and source-code
```javascript
function XMLComment(parent, text) {
  XMLComment.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing comment text");
  }
  this.text = this.stringify.comment(text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDTDAttList"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDAttList (parent, elementName, attributeName, attributeType, defaultValueType, defaultValue)](#apidoc.element.xmlbuilder.XMLDTDAttList)
- description and source-code
```javascript
function XMLDTDAttList(parent, elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  XMLDTDAttList.__super__.constructor.call(this, parent);
  if (elementName == null) {
    throw new Error("Missing DTD element name");
  }
  if (attributeName == null) {
    throw new Error("Missing DTD attribute name");
  }
  if (!attributeType) {
    throw new Error("Missing DTD attribute type");
  }
  if (!defaultValueType) {
    throw new Error("Missing DTD attribute default");
  }
  if (defaultValueType.indexOf('#') !== 0) {
    defaultValueType = '#' + defaultValueType;
  }
  if (!defaultValueType.match(/^(#REQUIRED|#IMPLIED|#FIXED|#DEFAULT)$/)) {
    throw new Error("Invalid default value type; expected: #REQUIRED, #IMPLIED, #FIXED or #DEFAULT");
  }
  if (defaultValue && !defaultValueType.match(/^(#FIXED|#DEFAULT)$/)) {
    throw new Error("Default value only applies to #FIXED or #DEFAULT");
  }
  this.elementName = this.stringify.eleName(elementName);
  this.attributeName = this.stringify.attName(attributeName);
  this.attributeType = this.stringify.dtdAttType(attributeType);
  this.defaultValue = this.stringify.dtdAttDefault(defaultValue);
  this.defaultValueType = defaultValueType;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDTDElement"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDElement (parent, name, value)](#apidoc.element.xmlbuilder.XMLDTDElement)
- description and source-code
```javascript
function XMLDTDElement(parent, name, value) {
  XMLDTDElement.__super__.constructor.call(this, parent);
  if (name == null) {
    throw new Error("Missing DTD element name");
  }
  if (!value) {
    value = '(#PCDATA)';
  }
  if (Array.isArray(value)) {
    value = '(' + value.join(',') + ')';
  }
  this.name = this.stringify.eleName(name);
  this.value = this.stringify.dtdElementValue(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDTDEntity"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDEntity (parent, pe, name, value)](#apidoc.element.xmlbuilder.XMLDTDEntity)
- description and source-code
```javascript
function XMLDTDEntity(parent, pe, name, value) {
  XMLDTDEntity.__super__.constructor.call(this, parent);
  if (name == null) {
    throw new Error("Missing entity name");
  }
  if (value == null) {
    throw new Error("Missing entity value");
  }
  this.pe = !!pe;
  this.name = this.stringify.eleName(name);
  if (!isObject(value)) {
    this.value = this.stringify.dtdEntityValue(value);
  } else {
    if (!value.pubID && !value.sysID) {
      throw new Error("Public and/or system identifiers are required for an external entity");
    }
    if (value.pubID && !value.sysID) {
      throw new Error("System identifier is required for a public external entity");
    }
    if (value.pubID != null) {
      this.pubID = this.stringify.dtdPubID(value.pubID);
    }
    if (value.sysID != null) {
      this.sysID = this.stringify.dtdSysID(value.sysID);
    }
    if (value.nData != null) {
      this.nData = this.stringify.dtdNData(value.nData);
    }
    if (this.pe && this.nData) {
      throw new Error("Notation declaration is not allowed in a parameter entity");
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDTDNotation"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDNotation (parent, name, value)](#apidoc.element.xmlbuilder.XMLDTDNotation)
- description and source-code
```javascript
function XMLDTDNotation(parent, name, value) {
  XMLDTDNotation.__super__.constructor.call(this, parent);
  if (name == null) {
    throw new Error("Missing notation name");
  }
  if (!value.pubID && !value.sysID) {
    throw new Error("Public or system identifiers are required for an external entity");
  }
  this.name = this.stringify.eleName(name);
  if (value.pubID != null) {
    this.pubID = this.stringify.dtdPubID(value.pubID);
  }
  if (value.sysID != null) {
    this.sysID = this.stringify.dtdSysID(value.sysID);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDeclaration"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDeclaration (parent, version, encoding, standalone)](#apidoc.element.xmlbuilder.XMLDeclaration)
- description and source-code
```javascript
function XMLDeclaration(parent, version, encoding, standalone) {
  var ref;
  XMLDeclaration.__super__.constructor.call(this, parent);
  if (isObject(version)) {
    ref = version, version = ref.version, encoding = ref.encoding, standalone = ref.standalone;
  }
  if (!version) {
    version = '1.0';
  }
  this.version = this.stringify.xmlVersion(version);
  if (encoding != null) {
    this.encoding = this.stringify.xmlEncoding(encoding);
  }
  if (standalone != null) {
    this.standalone = this.stringify.xmlStandalone(standalone);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocType"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocType (parent, pubID, sysID)](#apidoc.element.xmlbuilder.XMLDocType)
- description and source-code
```javascript
function XMLDocType(parent, pubID, sysID) {
  var ref, ref1;
  XMLDocType.__super__.constructor.call(this, parent);
  this.documentObject = parent;
  if (isObject(pubID)) {
    ref = pubID, pubID = ref.pubID, sysID = ref.sysID;
  }
  if (sysID == null) {
    ref1 = [pubID, sysID], sysID = ref1[0], pubID = ref1[1];
  }
  if (pubID != null) {
    this.pubID = this.stringify.dtdPubID(pubID);
  }
  if (sysID != null) {
    this.sysID = this.stringify.dtdSysID(sysID);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocument"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocument (options)](#apidoc.element.xmlbuilder.XMLDocument)
- description and source-code
```javascript
function XMLDocument(options) {
  XMLDocument.__super__.constructor.call(this, null);
  options || (options = {});
  if (!options.writer) {
    options.writer = new XMLStringWriter();
  }
  this.options = options;
  this.stringify = new XMLStringifier(options);
  this.isDocument = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocumentCB (options, onData, onEnd)](#apidoc.element.xmlbuilder.XMLDocumentCB)
- description and source-code
```javascript
function XMLDocumentCB(options, onData, onEnd) {
  var writerOptions;
  options || (options = {});
  if (!options.writer) {
    options.writer = new XMLStringWriter(options);
  } else if (isPlainObject(options.writer)) {
    writerOptions = options.writer;
    options.writer = new XMLStringWriter(writerOptions);
  }
  this.options = options;
  this.writer = options.writer;
  this.stringify = new XMLStringifier(options);
  this.onDataCallback = onData || function() {};
  this.onEndCallback = onEnd || function() {};
  this.currentNode = null;
  this.currentLevel = -1;
  this.openTags = {};
  this.documentStarted = false;
  this.documentCompleted = false;
  this.root = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLElement"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLElement (parent, name, attributes)](#apidoc.element.xmlbuilder.XMLElement)
- description and source-code
```javascript
function XMLElement(parent, name, attributes) {
  XMLElement.__super__.constructor.call(this, parent);
  if (name == null) {
    throw new Error("Missing element name");
  }
  this.name = this.stringify.eleName(name);
  this.attributes = {};
  if (attributes != null) {
    this.attribute(attributes);
  }
  if (parent.isDocument) {
    this.isRoot = true;
    this.documentObject = parent;
    parent.rootObject = this;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLNode (parent)](#apidoc.element.xmlbuilder.XMLNode)
- description and source-code
```javascript
function XMLNode(parent) {
  this.parent = parent;
  if (this.parent) {
    this.options = this.parent.options;
    this.stringify = this.parent.stringify;
  }
  this.children = [];
  if (!XMLElement) {
    XMLElement = require('./XMLElement');
    XMLCData = require('./XMLCData');
    XMLComment = require('./XMLComment');
    XMLDeclaration = require('./XMLDeclaration');
    XMLDocType = require('./XMLDocType');
    XMLRaw = require('./XMLRaw');
    XMLText = require('./XMLText');
    XMLProcessingInstruction = require('./XMLProcessingInstruction');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLProcessingInstruction"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLProcessingInstruction (parent, target, value)](#apidoc.element.xmlbuilder.XMLProcessingInstruction)
- description and source-code
```javascript
function XMLProcessingInstruction(parent, target, value) {
  XMLProcessingInstruction.__super__.constructor.call(this, parent);
  if (target == null) {
    throw new Error("Missing instruction target");
  }
  this.target = this.stringify.insTarget(target);
  if (value) {
    this.value = this.stringify.insValue(value);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLRaw"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLRaw (parent, text)](#apidoc.element.xmlbuilder.XMLRaw)
- description and source-code
```javascript
function XMLRaw(parent, text) {
  XMLRaw.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing raw text");
  }
  this.value = this.stringify.raw(text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStreamWriter (stream, options)](#apidoc.element.xmlbuilder.XMLStreamWriter)
- description and source-code
```javascript
function XMLStreamWriter(stream, options) {
  this.stream = stream;
  XMLStreamWriter.__super__.constructor.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStringWriter (options)](#apidoc.element.xmlbuilder.XMLStringWriter)
- description and source-code
```javascript
function XMLStringWriter(options) {
  XMLStringWriter.__super__.constructor.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStringifier (options)](#apidoc.element.xmlbuilder.XMLStringifier)
- description and source-code
```javascript
function XMLStringifier(options) {
  this.assertLegalChar = bind(this.assertLegalChar, this);
  var key, ref1, value;
  options || (options = {});
  this.allowSurrogateChars = options.allowSurrogateChars;
  this.noDoubleEncoding = options.noDoubleEncoding;
  this.textCase = options.textCase;
  ref1 = options.stringify || {};
  for (key in ref1) {
    if (!hasProp.call(ref1, key)) continue;
    value = ref1[key];
    this[key] = value;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLText"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLText (parent, text)](#apidoc.element.xmlbuilder.XMLText)
- description and source-code
```javascript
function XMLText(parent, text) {
  XMLText.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing element text");
  }
  this.value = this.stringify.eleText(text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLWriterBase"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLWriterBase (options)](#apidoc.element.xmlbuilder.XMLWriterBase)
- description and source-code
```javascript
function XMLWriterBase(options) {
  var key, ref, ref1, ref2, ref3, ref4, value;
  options || (options = {});
  this.pretty = options.pretty || false;
  this.allowEmpty = (ref = options.allowEmpty) != null ? ref : false;
  if (this.pretty) {
    this.indent = (ref1 = options.indent) != null ? ref1 : '  ';
    this.newline = (ref2 = options.newline) != null ? ref2 : '\n';
    this.offset = (ref3 = options.offset) != null ? ref3 : 0;
  } else {
    this.indent = '';
    this.newline = '';
    this.offset = 0;
  }
  ref4 = options.writer || {};
  for (key in ref4) {
    if (!hasProp.call(ref4, key)) continue;
    value = ref4[key];
    this[key] = value;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.begin"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>begin (options, onData, onEnd)](#apidoc.element.xmlbuilder.begin)
- description and source-code
```javascript
begin = function (options, onData, onEnd) {
  var ref1;
  if (isFunction(options)) {
    ref1 = [options, onData], onData = ref1[0], onEnd = ref1[1];
    options = {};
  }
  if (onData) {
    return new XMLDocumentCB(options, onData, onEnd);
  } else {
    return new XMLDocument(options);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.create"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>create (name, xmldec, doctype, options)](#apidoc.element.xmlbuilder.create)
- description and source-code
```javascript
create = function (name, xmldec, doctype, options) {
  var doc, root;
  if (name == null) {
    throw new Error("Root element needs a name");
  }
  options = assign({}, xmldec, doctype, options);
  doc = new XMLDocument(options);
  root = doc.element(name);
  if (!options.headless) {
    doc.declaration(options);
    if ((options.pubID != null) || (options.sysID != null)) {
      doc.doctype(options);
    }
  }
  return root;
}
```
- example usage
```shell
...
npm install xmlbuilder
'''

### Usage:

''' js
var builder = require('xmlbuilder');
var xml = builder.create('root')
  .ele('xmlbuilder')
    .ele('repo', {'type': 'git'}, 'git://github.com/oozcitak/xmlbuilder-js.git')
  .end({ pretty: true});

console.log(xml);
'''
...
```

#### <a name="apidoc.element.xmlbuilder.streamWriter"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>streamWriter (stream, options)](#apidoc.element.xmlbuilder.streamWriter)
- description and source-code
```javascript
streamWriter = function (stream, options) {
  return new XMLStreamWriter(stream, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.stringWriter"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>stringWriter (options)](#apidoc.element.xmlbuilder.stringWriter)
- description and source-code
```javascript
stringWriter = function (options) {
  return new XMLStringWriter(options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.Utility"></a>[module xmlbuilder.Utility](#apidoc.module.xmlbuilder.Utility)

#### <a name="apidoc.element.xmlbuilder.Utility.assign"></a>[function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>assign ()](#apidoc.element.xmlbuilder.Utility.assign)
- description and source-code
```javascript
assign = function () {
  var i, key, len, source, sources, target;
  target = arguments[0], sources = 2 <= arguments.length ? slice.call(arguments, 1) : [];
  if (isFunction(Object.assign)) {
    Object.assign.apply(null, arguments);
  } else {
    for (i = 0, len = sources.length; i < len; i++) {
      source = sources[i];
      if (source != null) {
        for (key in source) {
          if (!hasProp.call(source, key)) continue;
          target[key] = source[key];
        }
      }
    }
  }
  return target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.Utility.camelCase"></a>[function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>camelCase (val)](#apidoc.element.xmlbuilder.Utility.camelCase)
- description and source-code
```javascript
camelCase = function (val) {
  var i, index, len, r, ref, word;
  r = '';
  ref = words(val);
  for (index = i = 0, len = ref.length; i < len; index = ++i) {
    word = ref[index];
    r += index ? capitalize(word.toLowerCase()) : word.toLowerCase();
  }
  return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.Utility.capitalize"></a>[function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>capitalize (val)](#apidoc.element.xmlbuilder.Utility.capitalize)
- description and source-code
```javascript
capitalize = function (val) {
  return val.charAt(0).toUpperCase() + val.slice(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.Utility.isArray"></a>[function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>isArray (val)](#apidoc.element.xmlbuilder.Utility.isArray)
- description and source-code
```javascript
isArray = function (val) {
  if (isFunction(Array.isArray)) {
    return Array.isArray(val);
  } else {
    return Object.prototype.toString.call(val) === '[object Array]';
  }
}
```
- example usage
```shell
...
isObject = function(val) {
  var ref;
  return !!val && ((ref = typeof val) === 'function' || ref === 'object');
};

isArray = function(val) {
  if (isFunction(Array.isArray)) {
    return Array.isArray(val);
  } else {
    return Object.prototype.toString.call(val) === '[object Array]';
  }
};

isEmpty = function(val) {
  var key;
...
```

#### <a name="apidoc.element.xmlbuilder.Utility.isEmpty"></a>[function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>isEmpty (val)](#apidoc.element.xmlbuilder.Utility.isEmpty)
- description and source-code
```javascript
isEmpty = function (val) {
  var key;
  if (isArray(val)) {
    return !val.length;
  } else {
    for (key in val) {
      if (!hasProp.call(val, key)) continue;
      return false;
    }
    return true;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.Utility.isFunction"></a>[function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>isFunction (val)](#apidoc.element.xmlbuilder.Utility.isFunction)
- description and source-code
```javascript
isFunction = function (val) {
  return !!val && Object.prototype.toString.call(val) === '[object Function]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.Utility.isObject"></a>[function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>isObject (val)](#apidoc.element.xmlbuilder.Utility.isObject)
- description and source-code
```javascript
isObject = function (val) {
  var ref;
  return !!val && ((ref = typeof val) === 'function' || ref === 'object');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.Utility.isPlainObject"></a>[function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>isPlainObject (val)](#apidoc.element.xmlbuilder.Utility.isPlainObject)
- description and source-code
```javascript
isPlainObject = function (val) {
  var ctor, proto;
  return isObject(val) && (proto = Object.getPrototypeOf(val)) && (ctor = proto.constructor) && (typeof ctor === 'function') && (
ctor instanceof ctor) && (Function.prototype.toString.call(ctor) === Function.prototype.toString.call(Object));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.Utility.kebabCase"></a>[function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>kebabCase (val)](#apidoc.element.xmlbuilder.Utility.kebabCase)
- description and source-code
```javascript
kebabCase = function (val) {
  var i, index, len, r, ref, word;
  r = '';
  ref = words(val);
  for (index = i = 0, len = ref.length; i < len; index = ++i) {
    word = ref[index];
    r += (index ? '-' : '') + word.toLowerCase();
  }
  return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.Utility.snakeCase"></a>[function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>snakeCase (val)](#apidoc.element.xmlbuilder.Utility.snakeCase)
- description and source-code
```javascript
snakeCase = function (val) {
  var i, index, len, r, ref, word;
  r = '';
  ref = words(val);
  for (index = i = 0, len = ref.length; i < len; index = ++i) {
    word = ref[index];
    r += (index ? '_' : '') + word.toLowerCase();
  }
  return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.Utility.titleCase"></a>[function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>titleCase (val)](#apidoc.element.xmlbuilder.Utility.titleCase)
- description and source-code
```javascript
titleCase = function (val) {
  var i, index, len, r, ref, word;
  r = '';
  ref = words(val);
  for (index = i = 0, len = ref.length; i < len; index = ++i) {
    word = ref[index];
    r += capitalize(word.toLowerCase());
  }
  return r;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.Utility.words"></a>[function <span class="apidocSignatureSpan">xmlbuilder.Utility.</span>words (val)](#apidoc.element.xmlbuilder.Utility.words)
- description and source-code
```javascript
words = function (val) {
  return (val.split(/[-_\s]+|(?=[A-Z][a-z])/) || []).filter(function(n) {
    return !!n;
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLAttribute"></a>[module xmlbuilder.XMLAttribute](#apidoc.module.xmlbuilder.XMLAttribute)

#### <a name="apidoc.element.xmlbuilder.XMLAttribute.XMLAttribute"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLAttribute (parent, name, value)](#apidoc.element.xmlbuilder.XMLAttribute.XMLAttribute)
- description and source-code
```javascript
function XMLAttribute(parent, name, value) {
  this.options = parent.options;
  this.stringify = parent.stringify;
  if (name == null) {
    throw new Error("Missing attribute name of element " + parent.name);
  }
  if (value == null) {
    throw new Error("Missing attribute value for attribute " + name + " of element " + parent.name);
  }
  this.name = this.stringify.attName(name);
  this.value = this.stringify.attValue(value);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLAttribute.prototype"></a>[module xmlbuilder.XMLAttribute.prototype](#apidoc.module.xmlbuilder.XMLAttribute.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLAttribute.prototype.clone"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLAttribute.prototype.</span>clone ()](#apidoc.element.xmlbuilder.XMLAttribute.prototype.clone)
- description and source-code
```javascript
clone = function () {
  return Object.create(this);
}
```
- example usage
```shell
...
  clonedSelf.documentObject = null;
}
clonedSelf.attributes = {};
ref1 = this.attributes;
for (attName in ref1) {
  if (!hasProp.call(ref1, attName)) continue;
  att = ref1[attName];
  clonedSelf.attributes[attName] = att.clone();
}
clonedSelf.children = [];
this.children.forEach(function(child) {
  var clonedChild;
  clonedChild = child.clone();
  clonedChild.parent = clonedSelf;
  return clonedSelf.children.push(clonedChild);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLAttribute.prototype.toString"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLAttribute.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLAttribute.prototype.toString)
- description and source-code
```javascript
toString = function (options) {
  return this.options.writer.set(options).attribute(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLCData"></a>[module xmlbuilder.XMLCData](#apidoc.module.xmlbuilder.XMLCData)

#### <a name="apidoc.element.xmlbuilder.XMLCData.XMLCData"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLCData (parent, text)](#apidoc.element.xmlbuilder.XMLCData.XMLCData)
- description and source-code
```javascript
function XMLCData(parent, text) {
  XMLCData.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing CDATA text");
  }
  this.text = this.stringify.cdata(text);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLCData.prototype"></a>[module xmlbuilder.XMLCData.prototype](#apidoc.module.xmlbuilder.XMLCData.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLCData.prototype.clone"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLCData.prototype.</span>clone ()](#apidoc.element.xmlbuilder.XMLCData.prototype.clone)
- description and source-code
```javascript
clone = function () {
  return Object.create(this);
}
```
- example usage
```shell
...
  clonedSelf.documentObject = null;
}
clonedSelf.attributes = {};
ref1 = this.attributes;
for (attName in ref1) {
  if (!hasProp.call(ref1, attName)) continue;
  att = ref1[attName];
  clonedSelf.attributes[attName] = att.clone();
}
clonedSelf.children = [];
this.children.forEach(function(child) {
  var clonedChild;
  clonedChild = child.clone();
  clonedChild.parent = clonedSelf;
  return clonedSelf.children.push(clonedChild);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLCData.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLCData.prototype.</span>constructor (parent, text)](#apidoc.element.xmlbuilder.XMLCData.prototype.constructor)
- description and source-code
```javascript
function XMLCData(parent, text) {
  XMLCData.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing CDATA text");
  }
  this.text = this.stringify.cdata(text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLCData.prototype.toString"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLCData.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLCData.prototype.toString)
- description and source-code
```javascript
toString = function (options) {
  return this.options.writer.set(options).cdata(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLComment"></a>[module xmlbuilder.XMLComment](#apidoc.module.xmlbuilder.XMLComment)

#### <a name="apidoc.element.xmlbuilder.XMLComment.XMLComment"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLComment (parent, text)](#apidoc.element.xmlbuilder.XMLComment.XMLComment)
- description and source-code
```javascript
function XMLComment(parent, text) {
  XMLComment.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing comment text");
  }
  this.text = this.stringify.comment(text);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLComment.prototype"></a>[module xmlbuilder.XMLComment.prototype](#apidoc.module.xmlbuilder.XMLComment.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLComment.prototype.clone"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLComment.prototype.</span>clone ()](#apidoc.element.xmlbuilder.XMLComment.prototype.clone)
- description and source-code
```javascript
clone = function () {
  return Object.create(this);
}
```
- example usage
```shell
...
  clonedSelf.documentObject = null;
}
clonedSelf.attributes = {};
ref1 = this.attributes;
for (attName in ref1) {
  if (!hasProp.call(ref1, attName)) continue;
  att = ref1[attName];
  clonedSelf.attributes[attName] = att.clone();
}
clonedSelf.children = [];
this.children.forEach(function(child) {
  var clonedChild;
  clonedChild = child.clone();
  clonedChild.parent = clonedSelf;
  return clonedSelf.children.push(clonedChild);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLComment.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLComment.prototype.</span>constructor (parent, text)](#apidoc.element.xmlbuilder.XMLComment.prototype.constructor)
- description and source-code
```javascript
function XMLComment(parent, text) {
  XMLComment.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing comment text");
  }
  this.text = this.stringify.comment(text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLComment.prototype.toString"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLComment.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLComment.prototype.toString)
- description and source-code
```javascript
toString = function (options) {
  return this.options.writer.set(options).comment(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDTDAttList"></a>[module xmlbuilder.XMLDTDAttList](#apidoc.module.xmlbuilder.XMLDTDAttList)

#### <a name="apidoc.element.xmlbuilder.XMLDTDAttList.XMLDTDAttList"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDAttList (parent, elementName, attributeName, attributeType, defaultValueType, defaultValue)](#apidoc.element.xmlbuilder.XMLDTDAttList.XMLDTDAttList)
- description and source-code
```javascript
function XMLDTDAttList(parent, elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  XMLDTDAttList.__super__.constructor.call(this, parent);
  if (elementName == null) {
    throw new Error("Missing DTD element name");
  }
  if (attributeName == null) {
    throw new Error("Missing DTD attribute name");
  }
  if (!attributeType) {
    throw new Error("Missing DTD attribute type");
  }
  if (!defaultValueType) {
    throw new Error("Missing DTD attribute default");
  }
  if (defaultValueType.indexOf('#') !== 0) {
    defaultValueType = '#' + defaultValueType;
  }
  if (!defaultValueType.match(/^(#REQUIRED|#IMPLIED|#FIXED|#DEFAULT)$/)) {
    throw new Error("Invalid default value type; expected: #REQUIRED, #IMPLIED, #FIXED or #DEFAULT");
  }
  if (defaultValue && !defaultValueType.match(/^(#FIXED|#DEFAULT)$/)) {
    throw new Error("Default value only applies to #FIXED or #DEFAULT");
  }
  this.elementName = this.stringify.eleName(elementName);
  this.attributeName = this.stringify.attName(attributeName);
  this.attributeType = this.stringify.dtdAttType(attributeType);
  this.defaultValue = this.stringify.dtdAttDefault(defaultValue);
  this.defaultValueType = defaultValueType;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDTDAttList.prototype"></a>[module xmlbuilder.XMLDTDAttList.prototype](#apidoc.module.xmlbuilder.XMLDTDAttList.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLDTDAttList.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDAttList.prototype.</span>constructor (parent, elementName, attributeName, attributeType, defaultValueType, defaultValue)](#apidoc.element.xmlbuilder.XMLDTDAttList.prototype.constructor)
- description and source-code
```javascript
function XMLDTDAttList(parent, elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  XMLDTDAttList.__super__.constructor.call(this, parent);
  if (elementName == null) {
    throw new Error("Missing DTD element name");
  }
  if (attributeName == null) {
    throw new Error("Missing DTD attribute name");
  }
  if (!attributeType) {
    throw new Error("Missing DTD attribute type");
  }
  if (!defaultValueType) {
    throw new Error("Missing DTD attribute default");
  }
  if (defaultValueType.indexOf('#') !== 0) {
    defaultValueType = '#' + defaultValueType;
  }
  if (!defaultValueType.match(/^(#REQUIRED|#IMPLIED|#FIXED|#DEFAULT)$/)) {
    throw new Error("Invalid default value type; expected: #REQUIRED, #IMPLIED, #FIXED or #DEFAULT");
  }
  if (defaultValue && !defaultValueType.match(/^(#FIXED|#DEFAULT)$/)) {
    throw new Error("Default value only applies to #FIXED or #DEFAULT");
  }
  this.elementName = this.stringify.eleName(elementName);
  this.attributeName = this.stringify.attName(attributeName);
  this.attributeType = this.stringify.dtdAttType(attributeType);
  this.defaultValue = this.stringify.dtdAttDefault(defaultValue);
  this.defaultValueType = defaultValueType;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDTDAttList.prototype.toString"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDAttList.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLDTDAttList.prototype.toString)
- description and source-code
```javascript
toString = function (options) {
  return this.options.writer.set(options).dtdAttList(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDTDElement"></a>[module xmlbuilder.XMLDTDElement](#apidoc.module.xmlbuilder.XMLDTDElement)

#### <a name="apidoc.element.xmlbuilder.XMLDTDElement.XMLDTDElement"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDElement (parent, name, value)](#apidoc.element.xmlbuilder.XMLDTDElement.XMLDTDElement)
- description and source-code
```javascript
function XMLDTDElement(parent, name, value) {
  XMLDTDElement.__super__.constructor.call(this, parent);
  if (name == null) {
    throw new Error("Missing DTD element name");
  }
  if (!value) {
    value = '(#PCDATA)';
  }
  if (Array.isArray(value)) {
    value = '(' + value.join(',') + ')';
  }
  this.name = this.stringify.eleName(name);
  this.value = this.stringify.dtdElementValue(value);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDTDElement.prototype"></a>[module xmlbuilder.XMLDTDElement.prototype](#apidoc.module.xmlbuilder.XMLDTDElement.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLDTDElement.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDElement.prototype.</span>constructor (parent, name, value)](#apidoc.element.xmlbuilder.XMLDTDElement.prototype.constructor)
- description and source-code
```javascript
function XMLDTDElement(parent, name, value) {
  XMLDTDElement.__super__.constructor.call(this, parent);
  if (name == null) {
    throw new Error("Missing DTD element name");
  }
  if (!value) {
    value = '(#PCDATA)';
  }
  if (Array.isArray(value)) {
    value = '(' + value.join(',') + ')';
  }
  this.name = this.stringify.eleName(name);
  this.value = this.stringify.dtdElementValue(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDTDElement.prototype.toString"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDElement.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLDTDElement.prototype.toString)
- description and source-code
```javascript
toString = function (options) {
  return this.options.writer.set(options).dtdElement(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDTDEntity"></a>[module xmlbuilder.XMLDTDEntity](#apidoc.module.xmlbuilder.XMLDTDEntity)

#### <a name="apidoc.element.xmlbuilder.XMLDTDEntity.XMLDTDEntity"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDEntity (parent, pe, name, value)](#apidoc.element.xmlbuilder.XMLDTDEntity.XMLDTDEntity)
- description and source-code
```javascript
function XMLDTDEntity(parent, pe, name, value) {
  XMLDTDEntity.__super__.constructor.call(this, parent);
  if (name == null) {
    throw new Error("Missing entity name");
  }
  if (value == null) {
    throw new Error("Missing entity value");
  }
  this.pe = !!pe;
  this.name = this.stringify.eleName(name);
  if (!isObject(value)) {
    this.value = this.stringify.dtdEntityValue(value);
  } else {
    if (!value.pubID && !value.sysID) {
      throw new Error("Public and/or system identifiers are required for an external entity");
    }
    if (value.pubID && !value.sysID) {
      throw new Error("System identifier is required for a public external entity");
    }
    if (value.pubID != null) {
      this.pubID = this.stringify.dtdPubID(value.pubID);
    }
    if (value.sysID != null) {
      this.sysID = this.stringify.dtdSysID(value.sysID);
    }
    if (value.nData != null) {
      this.nData = this.stringify.dtdNData(value.nData);
    }
    if (this.pe && this.nData) {
      throw new Error("Notation declaration is not allowed in a parameter entity");
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDTDEntity.prototype"></a>[module xmlbuilder.XMLDTDEntity.prototype](#apidoc.module.xmlbuilder.XMLDTDEntity.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLDTDEntity.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDEntity.prototype.</span>constructor (parent, pe, name, value)](#apidoc.element.xmlbuilder.XMLDTDEntity.prototype.constructor)
- description and source-code
```javascript
function XMLDTDEntity(parent, pe, name, value) {
  XMLDTDEntity.__super__.constructor.call(this, parent);
  if (name == null) {
    throw new Error("Missing entity name");
  }
  if (value == null) {
    throw new Error("Missing entity value");
  }
  this.pe = !!pe;
  this.name = this.stringify.eleName(name);
  if (!isObject(value)) {
    this.value = this.stringify.dtdEntityValue(value);
  } else {
    if (!value.pubID && !value.sysID) {
      throw new Error("Public and/or system identifiers are required for an external entity");
    }
    if (value.pubID && !value.sysID) {
      throw new Error("System identifier is required for a public external entity");
    }
    if (value.pubID != null) {
      this.pubID = this.stringify.dtdPubID(value.pubID);
    }
    if (value.sysID != null) {
      this.sysID = this.stringify.dtdSysID(value.sysID);
    }
    if (value.nData != null) {
      this.nData = this.stringify.dtdNData(value.nData);
    }
    if (this.pe && this.nData) {
      throw new Error("Notation declaration is not allowed in a parameter entity");
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDTDEntity.prototype.toString"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDEntity.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLDTDEntity.prototype.toString)
- description and source-code
```javascript
toString = function (options) {
  return this.options.writer.set(options).dtdEntity(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDTDNotation"></a>[module xmlbuilder.XMLDTDNotation](#apidoc.module.xmlbuilder.XMLDTDNotation)

#### <a name="apidoc.element.xmlbuilder.XMLDTDNotation.XMLDTDNotation"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDTDNotation (parent, name, value)](#apidoc.element.xmlbuilder.XMLDTDNotation.XMLDTDNotation)
- description and source-code
```javascript
function XMLDTDNotation(parent, name, value) {
  XMLDTDNotation.__super__.constructor.call(this, parent);
  if (name == null) {
    throw new Error("Missing notation name");
  }
  if (!value.pubID && !value.sysID) {
    throw new Error("Public or system identifiers are required for an external entity");
  }
  this.name = this.stringify.eleName(name);
  if (value.pubID != null) {
    this.pubID = this.stringify.dtdPubID(value.pubID);
  }
  if (value.sysID != null) {
    this.sysID = this.stringify.dtdSysID(value.sysID);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDTDNotation.prototype"></a>[module xmlbuilder.XMLDTDNotation.prototype](#apidoc.module.xmlbuilder.XMLDTDNotation.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLDTDNotation.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDNotation.prototype.</span>constructor (parent, name, value)](#apidoc.element.xmlbuilder.XMLDTDNotation.prototype.constructor)
- description and source-code
```javascript
function XMLDTDNotation(parent, name, value) {
  XMLDTDNotation.__super__.constructor.call(this, parent);
  if (name == null) {
    throw new Error("Missing notation name");
  }
  if (!value.pubID && !value.sysID) {
    throw new Error("Public or system identifiers are required for an external entity");
  }
  this.name = this.stringify.eleName(name);
  if (value.pubID != null) {
    this.pubID = this.stringify.dtdPubID(value.pubID);
  }
  if (value.sysID != null) {
    this.sysID = this.stringify.dtdSysID(value.sysID);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDTDNotation.prototype.toString"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDTDNotation.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLDTDNotation.prototype.toString)
- description and source-code
```javascript
toString = function (options) {
  return this.options.writer.set(options).dtdNotation(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDeclaration"></a>[module xmlbuilder.XMLDeclaration](#apidoc.module.xmlbuilder.XMLDeclaration)

#### <a name="apidoc.element.xmlbuilder.XMLDeclaration.XMLDeclaration"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDeclaration (parent, version, encoding, standalone)](#apidoc.element.xmlbuilder.XMLDeclaration.XMLDeclaration)
- description and source-code
```javascript
function XMLDeclaration(parent, version, encoding, standalone) {
  var ref;
  XMLDeclaration.__super__.constructor.call(this, parent);
  if (isObject(version)) {
    ref = version, version = ref.version, encoding = ref.encoding, standalone = ref.standalone;
  }
  if (!version) {
    version = '1.0';
  }
  this.version = this.stringify.xmlVersion(version);
  if (encoding != null) {
    this.encoding = this.stringify.xmlEncoding(encoding);
  }
  if (standalone != null) {
    this.standalone = this.stringify.xmlStandalone(standalone);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDeclaration.prototype"></a>[module xmlbuilder.XMLDeclaration.prototype](#apidoc.module.xmlbuilder.XMLDeclaration.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLDeclaration.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDeclaration.prototype.</span>constructor (parent, version, encoding, standalone)](#apidoc.element.xmlbuilder.XMLDeclaration.prototype.constructor)
- description and source-code
```javascript
function XMLDeclaration(parent, version, encoding, standalone) {
  var ref;
  XMLDeclaration.__super__.constructor.call(this, parent);
  if (isObject(version)) {
    ref = version, version = ref.version, encoding = ref.encoding, standalone = ref.standalone;
  }
  if (!version) {
    version = '1.0';
  }
  this.version = this.stringify.xmlVersion(version);
  if (encoding != null) {
    this.encoding = this.stringify.xmlEncoding(encoding);
  }
  if (standalone != null) {
    this.standalone = this.stringify.xmlStandalone(standalone);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDeclaration.prototype.toString"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDeclaration.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLDeclaration.prototype.toString)
- description and source-code
```javascript
toString = function (options) {
  return this.options.writer.set(options).declaration(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDocType"></a>[module xmlbuilder.XMLDocType](#apidoc.module.xmlbuilder.XMLDocType)

#### <a name="apidoc.element.xmlbuilder.XMLDocType.XMLDocType"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocType (parent, pubID, sysID)](#apidoc.element.xmlbuilder.XMLDocType.XMLDocType)
- description and source-code
```javascript
function XMLDocType(parent, pubID, sysID) {
  var ref, ref1;
  XMLDocType.__super__.constructor.call(this, parent);
  this.documentObject = parent;
  if (isObject(pubID)) {
    ref = pubID, pubID = ref.pubID, sysID = ref.sysID;
  }
  if (sysID == null) {
    ref1 = [pubID, sysID], sysID = ref1[0], pubID = ref1[1];
  }
  if (pubID != null) {
    this.pubID = this.stringify.dtdPubID(pubID);
  }
  if (sysID != null) {
    this.sysID = this.stringify.dtdSysID(sysID);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDocType.prototype"></a>[module xmlbuilder.XMLDocType.prototype](#apidoc.module.xmlbuilder.XMLDocType.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLDocType.prototype.att"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>att (elementName, attributeName, attributeType, defaultValueType, defaultValue)](#apidoc.element.xmlbuilder.XMLDocType.prototype.att)
- description and source-code
```javascript
att = function (elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  return this.attList(elementName, attributeName, attributeType, defaultValueType, defaultValue);
}
```
- example usage
```shell
...

''' js
var root = builder.create('squares');
root.com('f(x) = x^2');
for(var i = 1; i <= 5; i++)
{
  var item = root.ele('data');
  item.att('x', i);
  item.att('y', i * i);
}
'''

This will result in:

''' xml
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocType.prototype.attList"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>attList (elementName, attributeName, attributeType, defaultValueType, defaultValue)](#apidoc.element.xmlbuilder.XMLDocType.prototype.attList)
- description and source-code
```javascript
attList = function (elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  var child;
  child = new XMLDTDAttList(this, elementName, attributeName, attributeType, defaultValueType, defaultValue);
  this.children.push(child);
  return this;
}
```
- example usage
```shell
...
};

XMLDocType.prototype.ele = function(name, value) {
  return this.element(name, value);
};

XMLDocType.prototype.att = function(elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  return this.attList(elementName, attributeName, attributeType, defaultValueType, defaultValue);
};

XMLDocType.prototype.ent = function(name, value) {
  return this.entity(name, value);
};

XMLDocType.prototype.pent = function(name, value) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocType.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>constructor (parent, pubID, sysID)](#apidoc.element.xmlbuilder.XMLDocType.prototype.constructor)
- description and source-code
```javascript
function XMLDocType(parent, pubID, sysID) {
  var ref, ref1;
  XMLDocType.__super__.constructor.call(this, parent);
  this.documentObject = parent;
  if (isObject(pubID)) {
    ref = pubID, pubID = ref.pubID, sysID = ref.sysID;
  }
  if (sysID == null) {
    ref1 = [pubID, sysID], sysID = ref1[0], pubID = ref1[1];
  }
  if (pubID != null) {
    this.pubID = this.stringify.dtdPubID(pubID);
  }
  if (sysID != null) {
    this.sysID = this.stringify.dtdSysID(sysID);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocType.prototype.ele"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>ele (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.ele)
- description and source-code
```javascript
ele = function (name, value) {
  return this.element(name, value);
}
```
- example usage
```shell
...
'''

### Usage:

''' js
var builder = require('xmlbuilder');
var xml = builder.create('root')
  .ele('xmlbuilder')
    .ele('repo', {'type': 'git'}, 'git://github.com/oozcitak/xmlbuilder-js.git')
  .end({ pretty: true});

console.log(xml);
'''

will result in:
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocType.prototype.element"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>element (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.element)
- description and source-code
```javascript
element = function (name, value) {
  var child;
  child = new XMLDTDElement(this, name, value);
  this.children.push(child);
  return this;
}
```
- example usage
```shell
...
};

XMLDocType.prototype.toString = function(options) {
  return this.options.writer.set(options).docType(this);
};

XMLDocType.prototype.ele = function(name, value) {
  return this.element(name, value);
};

XMLDocType.prototype.att = function(elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  return this.attList(elementName, attributeName, attributeType, defaultValueType, defaultValue);
};

XMLDocType.prototype.ent = function(name, value) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocType.prototype.ent"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>ent (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.ent)
- description and source-code
```javascript
ent = function (name, value) {
  return this.entity(name, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocType.prototype.entity"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>entity (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.entity)
- description and source-code
```javascript
entity = function (name, value) {
  var child;
  child = new XMLDTDEntity(this, false, name, value);
  this.children.push(child);
  return this;
}
```
- example usage
```shell
...
};

XMLDocType.prototype.att = function(elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  return this.attList(elementName, attributeName, attributeType, defaultValueType, defaultValue);
};

XMLDocType.prototype.ent = function(name, value) {
  return this.entity(name, value);
};

XMLDocType.prototype.pent = function(name, value) {
  return this.pEntity(name, value);
};

XMLDocType.prototype.not = function(name, value) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocType.prototype.not"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>not (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.not)
- description and source-code
```javascript
not = function (name, value) {
  return this.notation(name, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocType.prototype.notation"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>notation (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.notation)
- description and source-code
```javascript
notation = function (name, value) {
  var child;
  child = new XMLDTDNotation(this, name, value);
  this.children.push(child);
  return this;
}
```
- example usage
```shell
...
};

XMLDocType.prototype.pent = function(name, value) {
  return this.pEntity(name, value);
};

XMLDocType.prototype.not = function(name, value) {
  return this.notation(name, value);
};

XMLDocType.prototype.up = function() {
  return this.root() || this.documentObject;
};

return XMLDocType;
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocType.prototype.pEntity"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>pEntity (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.pEntity)
- description and source-code
```javascript
pEntity = function (name, value) {
  var child;
  child = new XMLDTDEntity(this, true, name, value);
  this.children.push(child);
  return this;
}
```
- example usage
```shell
...
};

XMLDocType.prototype.ent = function(name, value) {
  return this.entity(name, value);
};

XMLDocType.prototype.pent = function(name, value) {
  return this.pEntity(name, value);
};

XMLDocType.prototype.not = function(name, value) {
  return this.notation(name, value);
};

XMLDocType.prototype.up = function() {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocType.prototype.pent"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>pent (name, value)](#apidoc.element.xmlbuilder.XMLDocType.prototype.pent)
- description and source-code
```javascript
pent = function (name, value) {
  return this.pEntity(name, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocType.prototype.toString"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLDocType.prototype.toString)
- description and source-code
```javascript
toString = function (options) {
  return this.options.writer.set(options).docType(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocType.prototype.up"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocType.prototype.</span>up ()](#apidoc.element.xmlbuilder.XMLDocType.prototype.up)
- description and source-code
```javascript
up = function () {
  return this.root() || this.documentObject;
}
```
- example usage
```shell
...
  delete this.openTags[this.currentLevel];
  this.currentLevel--;
  return this;
};

XMLDocumentCB.prototype.end = function() {
  while (this.currentLevel >= 0) {
    this.up();
  }
  return this.onEnd();
};

XMLDocumentCB.prototype.openCurrent = function() {
  if (this.currentNode) {
    this.currentNode.children = true;
...
```



# <a name="apidoc.module.xmlbuilder.XMLDocument"></a>[module xmlbuilder.XMLDocument](#apidoc.module.xmlbuilder.XMLDocument)

#### <a name="apidoc.element.xmlbuilder.XMLDocument.XMLDocument"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocument (options)](#apidoc.element.xmlbuilder.XMLDocument.XMLDocument)
- description and source-code
```javascript
function XMLDocument(options) {
  XMLDocument.__super__.constructor.call(this, null);
  options || (options = {});
  if (!options.writer) {
    options.writer = new XMLStringWriter();
  }
  this.options = options;
  this.stringify = new XMLStringifier(options);
  this.isDocument = true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDocument.prototype"></a>[module xmlbuilder.XMLDocument.prototype](#apidoc.module.xmlbuilder.XMLDocument.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLDocument.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocument.prototype.</span>constructor (options)](#apidoc.element.xmlbuilder.XMLDocument.prototype.constructor)
- description and source-code
```javascript
function XMLDocument(options) {
  XMLDocument.__super__.constructor.call(this, null);
  options || (options = {});
  if (!options.writer) {
    options.writer = new XMLStringWriter();
  }
  this.options = options;
  this.stringify = new XMLStringifier(options);
  this.isDocument = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocument.prototype.end"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocument.prototype.</span>end (writer)](#apidoc.element.xmlbuilder.XMLDocument.prototype.end)
- description and source-code
```javascript
end = function (writer) {
  var writerOptions;
  if (!writer) {
    writer = this.options.writer;
  } else if (isPlainObject(writer)) {
    writerOptions = writer;
    writer = this.options.writer.set(writerOptions);
  }
  return writer.document(this);
}
```
- example usage
```shell
...
### Usage:

''' js
var builder = require('xmlbuilder');
var xml = builder.create('root')
  .ele('xmlbuilder')
    .ele('repo', {'type': 'git'}, 'git://github.com/oozcitak/xmlbuilder-js.git')
  .end({ pretty: true});

console.log(xml);
'''

will result in:

''' xml
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocument.prototype.toString"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocument.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLDocument.prototype.toString)
- description and source-code
```javascript
toString = function (options) {
  return this.options.writer.set(options).document(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDocumentCB"></a>[module xmlbuilder.XMLDocumentCB](#apidoc.module.xmlbuilder.XMLDocumentCB)

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.XMLDocumentCB"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLDocumentCB (options, onData, onEnd)](#apidoc.element.xmlbuilder.XMLDocumentCB.XMLDocumentCB)
- description and source-code
```javascript
function XMLDocumentCB(options, onData, onEnd) {
  var writerOptions;
  options || (options = {});
  if (!options.writer) {
    options.writer = new XMLStringWriter(options);
  } else if (isPlainObject(options.writer)) {
    writerOptions = options.writer;
    options.writer = new XMLStringWriter(writerOptions);
  }
  this.options = options;
  this.writer = options.writer;
  this.stringify = new XMLStringifier(options);
  this.onDataCallback = onData || function() {};
  this.onEndCallback = onEnd || function() {};
  this.currentNode = null;
  this.currentLevel = -1;
  this.openTags = {};
  this.documentStarted = false;
  this.documentCompleted = false;
  this.root = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLDocumentCB.prototype"></a>[module xmlbuilder.XMLDocumentCB.prototype](#apidoc.module.xmlbuilder.XMLDocumentCB.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.a"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>a ()](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.a)
- description and source-code
```javascript
a = function () {
  if (this.currentNode && this.currentNode instanceof XMLDocType) {
    return this.attList.apply(this, arguments);
  } else {
    return this.attribute.apply(this, arguments);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.att"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>att ()](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.att)
- description and source-code
```javascript
att = function () {
  if (this.currentNode && this.currentNode instanceof XMLDocType) {
    return this.attList.apply(this, arguments);
  } else {
    return this.attribute.apply(this, arguments);
  }
}
```
- example usage
```shell
...

''' js
var root = builder.create('squares');
root.com('f(x) = x^2');
for(var i = 1; i <= 5; i++)
{
  var item = root.ele('data');
  item.att('x', i);
  item.att('y', i * i);
}
'''

This will result in:

''' xml
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.attList"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>attList (elementName, attributeName, attributeType, defaultValueType, defaultValue)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.attList)
- description and source-code
```javascript
attList = function (elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  var node;
  this.openCurrent();
  node = new XMLDTDAttList(this, elementName, attributeName, attributeType, defaultValueType, defaultValue);
  this.onData(this.writer.dtdAttList(node, this.currentLevel + 1));
  return this;
}
```
- example usage
```shell
...
};

XMLDocType.prototype.ele = function(name, value) {
  return this.element(name, value);
};

XMLDocType.prototype.att = function(elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  return this.attList(elementName, attributeName, attributeType, defaultValueType, defaultValue);
};

XMLDocType.prototype.ent = function(name, value) {
  return this.entity(name, value);
};

XMLDocType.prototype.pent = function(name, value) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.attribute"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>attribute (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.attribute)
- description and source-code
```javascript
attribute = function (name, value) {
  var attName, attValue;
  if (!this.currentNode || this.currentNode.children) {
    throw new Error("att() can only be used immediately after an ele() call in callback mode");
  }
  if (name != null) {
    name = name.valueOf();
  }
  if (isObject(name)) {
    for (attName in name) {
      if (!hasProp.call(name, attName)) continue;
      attValue = name[attName];
      this.attribute(attName, attValue);
    }
  } else {
    if (isFunction(value)) {
      value = value.apply();
    }
    if (!this.options.skipNullAttributes || (value != null)) {
      this.currentNode.attributes[name] = new XMLAttribute(this, name, value);
    }
  }
  return this;
}
```
- example usage
```shell
...
    }

    XMLAttribute.prototype.clone = function() {
      return Object.create(this);
    };

    XMLAttribute.prototype.toString = function(options) {
      return this.options.writer.set(options).attribute(this);
    };

    return XMLAttribute;

  })();

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.c"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>c (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.c)
- description and source-code
```javascript
c = function (value) {
  return this.comment(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.cdata"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>cdata (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.cdata)
- description and source-code
```javascript
cdata = function (value) {
  var node;
  this.openCurrent();
  node = new XMLCData(this, value);
  this.onData(this.writer.cdata(node, this.currentLevel + 1));
  return this;
}
```
- example usage
```shell
...
extend(XMLCData, superClass);

function XMLCData(parent, text) {
  XMLCData.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing CDATA text");
  }
  this.text = this.stringify.cdata(text);
}

XMLCData.prototype.clone = function() {
  return Object.create(this);
};

XMLCData.prototype.toString = function(options) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.closeNode"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>closeNode (node)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.closeNode)
- description and source-code
```javascript
closeNode = function (node) {
  if (!node.isClosed) {
    this.onData(this.writer.closeNode(node, this.currentLevel));
    return node.isClosed = true;
  }
}
```
- example usage
```shell
...

    XMLDocumentCB.prototype.up = function() {
if (this.currentLevel < 0) {
  throw new Error("The document node has no parent");
}
if (this.currentNode) {
  if (this.currentNode.children) {
    this.closeNode(this.currentNode);
  } else {
    this.openNode(this.currentNode);
  }
  this.currentNode = null;
} else {
  this.closeNode(this.openTags[this.currentLevel]);
}
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.com"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>com (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.com)
- description and source-code
```javascript
com = function (value) {
  return this.comment(value);
}
```
- example usage
```shell
...
});
'''

If you need to do some processing:

''' js
var root = builder.create('squares');
root.com('f(x) = x^2');
for(var i = 1; i <= 5; i++)
{
  var item = root.ele('data');
  item.att('x', i);
  item.att('y', i * i);
}
'''
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.comment"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>comment (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.comment)
- description and source-code
```javascript
comment = function (value) {
  var node;
  this.openCurrent();
  node = new XMLComment(this, value);
  this.onData(this.writer.comment(node, this.currentLevel + 1));
  return this;
}
```
- example usage
```shell
...
extend(XMLComment, superClass);

function XMLComment(parent, text) {
  XMLComment.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing comment text");
  }
  this.text = this.stringify.comment(text);
}

XMLComment.prototype.clone = function() {
  return Object.create(this);
};

XMLComment.prototype.toString = function(options) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.d"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>d (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.d)
- description and source-code
```javascript
d = function (value) {
  return this.cdata(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.dat"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>dat (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.dat)
- description and source-code
```javascript
dat = function (value) {
  return this.cdata(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.dec"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>dec (version, encoding, standalone)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.dec)
- description and source-code
```javascript
dec = function (version, encoding, standalone) {
  return this.declaration(version, encoding, standalone);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.declaration"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>declaration (version, encoding, standalone)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.declaration)
- description and source-code
```javascript
declaration = function (version, encoding, standalone) {
  var node;
  this.openCurrent();
  if (this.documentStarted) {
    throw new Error("declaration() must be the first node");
  }
  node = new XMLDeclaration(this, version, encoding, standalone);
  this.onData(this.writer.declaration(node, this.currentLevel + 1));
  return this;
}
```
- example usage
```shell
...
      }
      if (standalone != null) {
        this.standalone = this.stringify.xmlStandalone(standalone);
      }
    }

    XMLDeclaration.prototype.toString = function(options) {
      return this.options.writer.set(options).declaration(this);
    };

    return XMLDeclaration;

  })(XMLNode);

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.doctype"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>doctype (root, pubID, sysID)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.doctype)
- description and source-code
```javascript
doctype = function (root, pubID, sysID) {
  this.openCurrent();
  if (root == null) {
    throw new Error("Missing root node name");
  }
  if (this.root) {
    throw new Error("dtd() must come before the root node");
  }
  this.currentNode = new XMLDocType(this, pubID, sysID);
  this.currentNode.rootNodeName = root;
  this.currentNode.children = false;
  this.currentLevel++;
  this.openTags[this.currentLevel] = this.currentNode;
  return this;
}
```
- example usage
```shell
...
};

XMLDocumentCB.prototype.dec = function(version, encoding, standalone) {
  return this.declaration(version, encoding, standalone);
};

XMLDocumentCB.prototype.dtd = function(root, pubID, sysID) {
  return this.doctype(root, pubID, sysID);
};

XMLDocumentCB.prototype.e = function(name, attributes, text) {
  return this.element(name, attributes, text);
};

XMLDocumentCB.prototype.n = function(name, attributes, text) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.dtd"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>dtd (root, pubID, sysID)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.dtd)
- description and source-code
```javascript
dtd = function (root, pubID, sysID) {
  return this.doctype(root, pubID, sysID);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.dtdElement"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>dtdElement (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.dtdElement)
- description and source-code
```javascript
dtdElement = function (name, value) {
  var node;
  this.openCurrent();
  node = new XMLDTDElement(this, name, value);
  this.onData(this.writer.dtdElement(node, this.currentLevel + 1));
  return this;
}
```
- example usage
```shell
...
        value = '(' + value.join(',') + ')';
      }
      this.name = this.stringify.eleName(name);
      this.value = this.stringify.dtdElementValue(value);
    }

    XMLDTDElement.prototype.toString = function(options) {
      return this.options.writer.set(options).dtdElement(this);
    };

    return XMLDTDElement;

  })(XMLNode);

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.e"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>e (name, attributes, text)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.e)
- description and source-code
```javascript
e = function (name, attributes, text) {
  return this.element(name, attributes, text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.ele"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>ele ()](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.ele)
- description and source-code
```javascript
ele = function () {
  return this.element.apply(this, arguments);
}
```
- example usage
```shell
...
'''

### Usage:

''' js
var builder = require('xmlbuilder');
var xml = builder.create('root')
  .ele('xmlbuilder')
    .ele('repo', {'type': 'git'}, 'git://github.com/oozcitak/xmlbuilder-js.git')
  .end({ pretty: true});

console.log(xml);
'''

will result in:
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.element"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>element (name, attributes, text)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.element)
- description and source-code
```javascript
element = function (name, attributes, text) {
  if (this.currentNode && this.currentNode instanceof XMLDocType) {
    return this.dtdElement.apply(this, arguments);
  } else {
    return this.node(name, attributes, text);
  }
}
```
- example usage
```shell
...
};

XMLDocType.prototype.toString = function(options) {
  return this.options.writer.set(options).docType(this);
};

XMLDocType.prototype.ele = function(name, value) {
  return this.element(name, value);
};

XMLDocType.prototype.att = function(elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  return this.attList(elementName, attributeName, attributeType, defaultValueType, defaultValue);
};

XMLDocType.prototype.ent = function(name, value) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.end"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>end ()](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.end)
- description and source-code
```javascript
end = function () {
  while (this.currentLevel >= 0) {
    this.up();
  }
  return this.onEnd();
}
```
- example usage
```shell
...
### Usage:

''' js
var builder = require('xmlbuilder');
var xml = builder.create('root')
  .ele('xmlbuilder')
    .ele('repo', {'type': 'git'}, 'git://github.com/oozcitak/xmlbuilder-js.git')
  .end({ pretty: true});

console.log(xml);
'''

will result in:

''' xml
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.ent"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>ent (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.ent)
- description and source-code
```javascript
ent = function (name, value) {
  return this.entity(name, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.entity"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>entity (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.entity)
- description and source-code
```javascript
entity = function (name, value) {
  var node;
  this.openCurrent();
  node = new XMLDTDEntity(this, false, name, value);
  this.onData(this.writer.dtdEntity(node, this.currentLevel + 1));
  return this;
}
```
- example usage
```shell
...
};

XMLDocType.prototype.att = function(elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  return this.attList(elementName, attributeName, attributeType, defaultValueType, defaultValue);
};

XMLDocType.prototype.ent = function(name, value) {
  return this.entity(name, value);
};

XMLDocType.prototype.pent = function(name, value) {
  return this.pEntity(name, value);
};

XMLDocType.prototype.not = function(name, value) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.i"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>i (target, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.i)
- description and source-code
```javascript
i = function (target, value) {
  return this.instruction(target, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.ins"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>ins (target, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.ins)
- description and source-code
```javascript
ins = function (target, value) {
  return this.instruction(target, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.instruction"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>instruction (target, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.instruction)
- description and source-code
```javascript
instruction = function (target, value) {
  var i, insTarget, insValue, len, node;
  this.openCurrent();
  if (target != null) {
    target = target.valueOf();
  }
  if (value != null) {
    value = value.valueOf();
  }
  if (Array.isArray(target)) {
    for (i = 0, len = target.length; i < len; i++) {
      insTarget = target[i];
      this.instruction(insTarget);
    }
  } else if (isObject(target)) {
    for (insTarget in target) {
      if (!hasProp.call(target, insTarget)) continue;
      insValue = target[insTarget];
      this.instruction(insTarget, insValue);
    }
  } else {
    if (isFunction(value)) {
      value = value.apply();
    }
    node = new XMLProcessingInstruction(this, target, value);
    this.onData(this.writer.processingInstruction(node, this.currentLevel + 1));
  }
  return this;
}
```
- example usage
```shell
...
}
if (value != null) {
  value = value.valueOf();
}
if (Array.isArray(target)) {
  for (i = 0, len = target.length; i < len; i++) {
    insTarget = target[i];
    this.instruction(insTarget);
  }
} else if (isObject(target)) {
  for (insTarget in target) {
    if (!hasProp.call(target, insTarget)) continue;
    insValue = target[insTarget];
    this.instruction(insTarget, insValue);
  }
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.n"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>n (name, attributes, text)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.n)
- description and source-code
```javascript
n = function (name, attributes, text) {
  return this.node(name, attributes, text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.nod"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>nod (name, attributes, text)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.nod)
- description and source-code
```javascript
nod = function (name, attributes, text) {
  return this.node(name, attributes, text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.node"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>node (name, attributes, text)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.node)
- description and source-code
```javascript
node = function (name, attributes, text) {
  var ref1;
  if (name == null) {
    throw new Error("Missing node name");
  }
  if (this.root && this.currentLevel === -1) {
    throw new Error("Document can only have one root node");
  }
  this.openCurrent();
  name = name.valueOf();
  if (attributes == null) {
    attributes = {};
  }
  attributes = attributes.valueOf();
  if (!isObject(attributes)) {
    ref1 = [attributes, text], text = ref1[0], attributes = ref1[1];
  }
  this.currentNode = new XMLElement(this, name, attributes);
  this.currentNode.children = false;
  this.currentLevel++;
  this.openTags[this.currentLevel] = this.currentNode;
  if (text != null) {
    this.text(text);
  }
  return this;
}
```
- example usage
```shell
...
  return this;
};

XMLDocumentCB.prototype.element = function(name, attributes, text) {
  if (this.currentNode && this.currentNode instanceof XMLDocType) {
    return this.dtdElement.apply(this, arguments);
  } else {
    return this.node(name, attributes, text);
  }
};

XMLDocumentCB.prototype.attribute = function(name, value) {
  var attName, attValue;
  if (!this.currentNode || this.currentNode.children) {
    throw new Error("att() can only be used immediately after an ele() call in callback mode");
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.not"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>not (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.not)
- description and source-code
```javascript
not = function (name, value) {
  return this.notation(name, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.notation"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>notation (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.notation)
- description and source-code
```javascript
notation = function (name, value) {
  var node;
  this.openCurrent();
  node = new XMLDTDNotation(this, name, value);
  this.onData(this.writer.dtdNotation(node, this.currentLevel + 1));
  return this;
}
```
- example usage
```shell
...
};

XMLDocType.prototype.pent = function(name, value) {
  return this.pEntity(name, value);
};

XMLDocType.prototype.not = function(name, value) {
  return this.notation(name, value);
};

XMLDocType.prototype.up = function() {
  return this.root() || this.documentObject;
};

return XMLDocType;
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.onData"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>onData (chunk)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.onData)
- description and source-code
```javascript
onData = function (chunk) {
  this.documentStarted = true;
  return this.onDataCallback(chunk);
}
```
- example usage
```shell
...
  return this;
};

XMLDocumentCB.prototype.text = function(value) {
  var node;
  this.openCurrent();
  node = new XMLText(this, value);
  this.onData(this.writer.text(node, this.currentLevel + 1));
  return this;
};

XMLDocumentCB.prototype.cdata = function(value) {
  var node;
  this.openCurrent();
  node = new XMLCData(this, value);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.onEnd"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>onEnd ()](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.onEnd)
- description and source-code
```javascript
onEnd = function () {
  this.documentCompleted = true;
  return this.onEndCallback();
}
```
- example usage
```shell
...
  return this;
};

XMLDocumentCB.prototype.end = function() {
  while (this.currentLevel >= 0) {
    this.up();
  }
  return this.onEnd();
};

XMLDocumentCB.prototype.openCurrent = function() {
  if (this.currentNode) {
    this.currentNode.children = true;
    return this.openNode(this.currentNode);
  }
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.openCurrent"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>openCurrent ()](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.openCurrent)
- description and source-code
```javascript
openCurrent = function () {
  if (this.currentNode) {
    this.currentNode.children = true;
    return this.openNode(this.currentNode);
  }
}
```
- example usage
```shell
...
var ref1;
if (name == null) {
  throw new Error("Missing node name");
}
if (this.root && this.currentLevel === -1) {
  throw new Error("Document can only have one root node");
}
this.openCurrent();
name = name.valueOf();
if (attributes == null) {
  attributes = {};
}
attributes = attributes.valueOf();
if (!isObject(attributes)) {
  ref1 = [attributes, text], text = ref1[0], attributes = ref1[1];
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.openNode"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>openNode (node)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.openNode)
- description and source-code
```javascript
openNode = function (node) {
  if (!node.isOpen) {
    if (!this.root && this.currentLevel === 0 && node instanceof XMLElement) {
      this.root = node;
    }
    this.onData(this.writer.openNode(node, this.currentLevel));
    return node.isOpen = true;
  }
}
```
- example usage
```shell
...
if (this.currentLevel < 0) {
  throw new Error("The document node has no parent");
}
if (this.currentNode) {
  if (this.currentNode.children) {
    this.closeNode(this.currentNode);
  } else {
    this.openNode(this.currentNode);
  }
  this.currentNode = null;
} else {
  this.closeNode(this.openTags[this.currentLevel]);
}
delete this.openTags[this.currentLevel];
this.currentLevel--;
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.pEntity"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>pEntity (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.pEntity)
- description and source-code
```javascript
pEntity = function (name, value) {
  var node;
  this.openCurrent();
  node = new XMLDTDEntity(this, true, name, value);
  this.onData(this.writer.dtdEntity(node, this.currentLevel + 1));
  return this;
}
```
- example usage
```shell
...
};

XMLDocType.prototype.ent = function(name, value) {
  return this.entity(name, value);
};

XMLDocType.prototype.pent = function(name, value) {
  return this.pEntity(name, value);
};

XMLDocType.prototype.not = function(name, value) {
  return this.notation(name, value);
};

XMLDocType.prototype.up = function() {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.pent"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>pent (name, value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.pent)
- description and source-code
```javascript
pent = function (name, value) {
  return this.pEntity(name, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.r"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>r (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.r)
- description and source-code
```javascript
r = function (value) {
  return this.raw(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.raw"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>raw (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.raw)
- description and source-code
```javascript
raw = function (value) {
  var node;
  this.openCurrent();
  node = new XMLRaw(this, value);
  this.onData(this.writer.raw(node, this.currentLevel + 1));
  return this;
}
```
- example usage
```shell
...
  return this;
};

XMLDocumentCB.prototype.raw = function(value) {
  var node;
  this.openCurrent();
  node = new XMLRaw(this, value);
  this.onData(this.writer.raw(node, this.currentLevel + 1));
  return this;
};

XMLDocumentCB.prototype.instruction = function(target, value) {
  var i, insTarget, insValue, len, node;
  this.openCurrent();
  if (target != null) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.t"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>t (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.t)
- description and source-code
```javascript
t = function (value) {
  return this.text(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.text"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>text (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.text)
- description and source-code
```javascript
text = function (value) {
  var node;
  this.openCurrent();
  node = new XMLText(this, value);
  this.onData(this.writer.text(node, this.currentLevel + 1));
  return this;
}
```
- example usage
```shell
...
    ref1 = [attributes, text], text = ref1[0], attributes = ref1[1];
  }
  this.currentNode = new XMLElement(this, name, attributes);
  this.currentNode.children = false;
  this.currentLevel++;
  this.openTags[this.currentLevel] = this.currentNode;
  if (text != null) {
    this.text(text);
  }
  return this;
};

XMLDocumentCB.prototype.element = function(name, attributes, text) {
  if (this.currentNode && this.currentNode instanceof XMLDocType) {
    return this.dtdElement.apply(this, arguments);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.txt"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>txt (value)](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.txt)
- description and source-code
```javascript
txt = function (value) {
  return this.text(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLDocumentCB.prototype.up"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLDocumentCB.prototype.</span>up ()](#apidoc.element.xmlbuilder.XMLDocumentCB.prototype.up)
- description and source-code
```javascript
up = function () {
  if (this.currentLevel < 0) {
    throw new Error("The document node has no parent");
  }
  if (this.currentNode) {
    if (this.currentNode.children) {
      this.closeNode(this.currentNode);
    } else {
      this.openNode(this.currentNode);
    }
    this.currentNode = null;
  } else {
    this.closeNode(this.openTags[this.currentLevel]);
  }
  delete this.openTags[this.currentLevel];
  this.currentLevel--;
  return this;
}
```
- example usage
```shell
...
  delete this.openTags[this.currentLevel];
  this.currentLevel--;
  return this;
};

XMLDocumentCB.prototype.end = function() {
  while (this.currentLevel >= 0) {
    this.up();
  }
  return this.onEnd();
};

XMLDocumentCB.prototype.openCurrent = function() {
  if (this.currentNode) {
    this.currentNode.children = true;
...
```



# <a name="apidoc.module.xmlbuilder.XMLElement"></a>[module xmlbuilder.XMLElement](#apidoc.module.xmlbuilder.XMLElement)

#### <a name="apidoc.element.xmlbuilder.XMLElement.XMLElement"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLElement (parent, name, attributes)](#apidoc.element.xmlbuilder.XMLElement.XMLElement)
- description and source-code
```javascript
function XMLElement(parent, name, attributes) {
  XMLElement.__super__.constructor.call(this, parent);
  if (name == null) {
    throw new Error("Missing element name");
  }
  this.name = this.stringify.eleName(name);
  this.attributes = {};
  if (attributes != null) {
    this.attribute(attributes);
  }
  if (parent.isDocument) {
    this.isRoot = true;
    this.documentObject = parent;
    parent.rootObject = this;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLElement.prototype"></a>[module xmlbuilder.XMLElement.prototype](#apidoc.module.xmlbuilder.XMLElement.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLElement.prototype.a"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLElement.prototype.</span>a (name, value)](#apidoc.element.xmlbuilder.XMLElement.prototype.a)
- description and source-code
```javascript
a = function (name, value) {
  return this.attribute(name, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLElement.prototype.att"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLElement.prototype.</span>att (name, value)](#apidoc.element.xmlbuilder.XMLElement.prototype.att)
- description and source-code
```javascript
att = function (name, value) {
  return this.attribute(name, value);
}
```
- example usage
```shell
...

''' js
var root = builder.create('squares');
root.com('f(x) = x^2');
for(var i = 1; i <= 5; i++)
{
  var item = root.ele('data');
  item.att('x', i);
  item.att('y', i * i);
}
'''

This will result in:

''' xml
...
```

#### <a name="apidoc.element.xmlbuilder.XMLElement.prototype.attribute"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLElement.prototype.</span>attribute (name, value)](#apidoc.element.xmlbuilder.XMLElement.prototype.attribute)
- description and source-code
```javascript
attribute = function (name, value) {
  var attName, attValue;
  if (name != null) {
    name = name.valueOf();
  }
  if (isObject(name)) {
    for (attName in name) {
      if (!hasProp.call(name, attName)) continue;
      attValue = name[attName];
      this.attribute(attName, attValue);
    }
  } else {
    if (isFunction(value)) {
      value = value.apply();
    }
    if (!this.options.skipNullAttributes || (value != null)) {
      this.attributes[name] = new XMLAttribute(this, name, value);
    }
  }
  return this;
}
```
- example usage
```shell
...
    }

    XMLAttribute.prototype.clone = function() {
      return Object.create(this);
    };

    XMLAttribute.prototype.toString = function(options) {
      return this.options.writer.set(options).attribute(this);
    };

    return XMLAttribute;

  })();

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLElement.prototype.clone"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLElement.prototype.</span>clone ()](#apidoc.element.xmlbuilder.XMLElement.prototype.clone)
- description and source-code
```javascript
clone = function () {
  var att, attName, clonedSelf, ref1;
  clonedSelf = Object.create(this);
  if (clonedSelf.isRoot) {
    clonedSelf.documentObject = null;
  }
  clonedSelf.attributes = {};
  ref1 = this.attributes;
  for (attName in ref1) {
    if (!hasProp.call(ref1, attName)) continue;
    att = ref1[attName];
    clonedSelf.attributes[attName] = att.clone();
  }
  clonedSelf.children = [];
  this.children.forEach(function(child) {
    var clonedChild;
    clonedChild = child.clone();
    clonedChild.parent = clonedSelf;
    return clonedSelf.children.push(clonedChild);
  });
  return clonedSelf;
}
```
- example usage
```shell
...
  clonedSelf.documentObject = null;
}
clonedSelf.attributes = {};
ref1 = this.attributes;
for (attName in ref1) {
  if (!hasProp.call(ref1, attName)) continue;
  att = ref1[attName];
  clonedSelf.attributes[attName] = att.clone();
}
clonedSelf.children = [];
this.children.forEach(function(child) {
  var clonedChild;
  clonedChild = child.clone();
  clonedChild.parent = clonedSelf;
  return clonedSelf.children.push(clonedChild);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLElement.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLElement.prototype.</span>constructor (parent, name, attributes)](#apidoc.element.xmlbuilder.XMLElement.prototype.constructor)
- description and source-code
```javascript
function XMLElement(parent, name, attributes) {
  XMLElement.__super__.constructor.call(this, parent);
  if (name == null) {
    throw new Error("Missing element name");
  }
  this.name = this.stringify.eleName(name);
  this.attributes = {};
  if (attributes != null) {
    this.attribute(attributes);
  }
  if (parent.isDocument) {
    this.isRoot = true;
    this.documentObject = parent;
    parent.rootObject = this;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLElement.prototype.removeAttribute"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLElement.prototype.</span>removeAttribute (name)](#apidoc.element.xmlbuilder.XMLElement.prototype.removeAttribute)
- description and source-code
```javascript
removeAttribute = function (name) {
  var attName, i, len;
  if (name == null) {
    throw new Error("Missing attribute name");
  }
  name = name.valueOf();
  if (Array.isArray(name)) {
    for (i = 0, len = name.length; i < len; i++) {
      attName = name[i];
      delete this.attributes[attName];
    }
  } else {
    delete this.attributes[name];
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLElement.prototype.toString"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLElement.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLElement.prototype.toString)
- description and source-code
```javascript
toString = function (options) {
  return this.options.writer.set(options).element(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLNode"></a>[module xmlbuilder.XMLNode](#apidoc.module.xmlbuilder.XMLNode)

#### <a name="apidoc.element.xmlbuilder.XMLNode.XMLNode"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLNode (parent)](#apidoc.element.xmlbuilder.XMLNode.XMLNode)
- description and source-code
```javascript
function XMLNode(parent) {
  this.parent = parent;
  if (this.parent) {
    this.options = this.parent.options;
    this.stringify = this.parent.stringify;
  }
  this.children = [];
  if (!XMLElement) {
    XMLElement = require('./XMLElement');
    XMLCData = require('./XMLCData');
    XMLComment = require('./XMLComment');
    XMLDeclaration = require('./XMLDeclaration');
    XMLDocType = require('./XMLDocType');
    XMLRaw = require('./XMLRaw');
    XMLText = require('./XMLText');
    XMLProcessingInstruction = require('./XMLProcessingInstruction');
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLNode.prototype"></a>[module xmlbuilder.XMLNode.prototype](#apidoc.module.xmlbuilder.XMLNode.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.c"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>c (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.c)
- description and source-code
```javascript
c = function (value) {
  return this.comment(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.cdata"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>cdata (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.cdata)
- description and source-code
```javascript
cdata = function (value) {
  var child;
  child = new XMLCData(this, value);
  this.children.push(child);
  return this;
}
```
- example usage
```shell
...
extend(XMLCData, superClass);

function XMLCData(parent, text) {
  XMLCData.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing CDATA text");
  }
  this.text = this.stringify.cdata(text);
}

XMLCData.prototype.clone = function() {
  return Object.create(this);
};

XMLCData.prototype.toString = function(options) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.com"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>com (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.com)
- description and source-code
```javascript
com = function (value) {
  return this.comment(value);
}
```
- example usage
```shell
...
});
'''

If you need to do some processing:

''' js
var root = builder.create('squares');
root.com('f(x) = x^2');
for(var i = 1; i <= 5; i++)
{
  var item = root.ele('data');
  item.att('x', i);
  item.att('y', i * i);
}
'''
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.comment"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>comment (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.comment)
- description and source-code
```javascript
comment = function (value) {
  var child;
  child = new XMLComment(this, value);
  this.children.push(child);
  return this;
}
```
- example usage
```shell
...
extend(XMLComment, superClass);

function XMLComment(parent, text) {
  XMLComment.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing comment text");
  }
  this.text = this.stringify.comment(text);
}

XMLComment.prototype.clone = function() {
  return Object.create(this);
};

XMLComment.prototype.toString = function(options) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.commentAfter"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>commentAfter (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.commentAfter)
- description and source-code
```javascript
commentAfter = function (value) {
  var child, i, removed;
  i = this.parent.children.indexOf(this);
  removed = this.parent.children.splice(i + 1);
  child = this.parent.comment(value);
  Array.prototype.push.apply(this.parent.children, removed);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.commentBefore"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>commentBefore (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.commentBefore)
- description and source-code
```javascript
commentBefore = function (value) {
  var child, i, removed;
  i = this.parent.children.indexOf(this);
  removed = this.parent.children.splice(i);
  child = this.parent.comment(value);
  Array.prototype.push.apply(this.parent.children, removed);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.d"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>d (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.d)
- description and source-code
```javascript
d = function (value) {
  return this.cdata(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.dat"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>dat (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.dat)
- description and source-code
```javascript
dat = function (value) {
  return this.cdata(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.dec"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>dec (version, encoding, standalone)](#apidoc.element.xmlbuilder.XMLNode.prototype.dec)
- description and source-code
```javascript
dec = function (version, encoding, standalone) {
  return this.declaration(version, encoding, standalone);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.declaration"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>declaration (version, encoding, standalone)](#apidoc.element.xmlbuilder.XMLNode.prototype.declaration)
- description and source-code
```javascript
declaration = function (version, encoding, standalone) {
  var doc, xmldec;
  doc = this.document();
  xmldec = new XMLDeclaration(doc, version, encoding, standalone);
  if (doc.children[0] instanceof XMLDeclaration) {
    doc.children[0] = xmldec;
  } else {
    doc.children.unshift(xmldec);
  }
  return doc.root() || doc;
}
```
- example usage
```shell
...
      }
      if (standalone != null) {
        this.standalone = this.stringify.xmlStandalone(standalone);
      }
    }

    XMLDeclaration.prototype.toString = function(options) {
      return this.options.writer.set(options).declaration(this);
    };

    return XMLDeclaration;

  })(XMLNode);

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.doc"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>doc ()](#apidoc.element.xmlbuilder.XMLNode.prototype.doc)
- description and source-code
```javascript
doc = function () {
  return this.document();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.doctype"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>doctype (pubID, sysID)](#apidoc.element.xmlbuilder.XMLNode.prototype.doctype)
- description and source-code
```javascript
doctype = function (pubID, sysID) {
  var child, doc, doctype, i, j, k, len, len1, ref1, ref2;
  doc = this.document();
  doctype = new XMLDocType(doc, pubID, sysID);
  ref1 = doc.children;
  for (i = j = 0, len = ref1.length; j < len; i = ++j) {
    child = ref1[i];
    if (child instanceof XMLDocType) {
      doc.children[i] = doctype;
      return doctype;
    }
  }
  ref2 = doc.children;
  for (i = k = 0, len1 = ref2.length; k < len1; i = ++k) {
    child = ref2[i];
    if (child.isRoot) {
      doc.children.splice(i, 0, doctype);
      return doctype;
    }
  }
  doc.children.push(doctype);
  return doctype;
}
```
- example usage
```shell
...
};

XMLDocumentCB.prototype.dec = function(version, encoding, standalone) {
  return this.declaration(version, encoding, standalone);
};

XMLDocumentCB.prototype.dtd = function(root, pubID, sysID) {
  return this.doctype(root, pubID, sysID);
};

XMLDocumentCB.prototype.e = function(name, attributes, text) {
  return this.element(name, attributes, text);
};

XMLDocumentCB.prototype.n = function(name, attributes, text) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.document"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>document ()](#apidoc.element.xmlbuilder.XMLNode.prototype.document)
- description and source-code
```javascript
document = function () {
  var node;
  node = this;
  while (node) {
    if (node.isDocument) {
      return node;
    } else {
      node = node.parent;
    }
  }
}
```
- example usage
```shell
...
  var writerOptions;
  if (!writer) {
    writer = this.options.writer;
  } else if (isPlainObject(writer)) {
    writerOptions = writer;
    writer = this.options.writer.set(writerOptions);
  }
  return writer.document(this);
};

XMLDocument.prototype.toString = function(options) {
  return this.options.writer.set(options).document(this);
};

return XMLDocument;
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.dtd"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>dtd (pubID, sysID)](#apidoc.element.xmlbuilder.XMLNode.prototype.dtd)
- description and source-code
```javascript
dtd = function (pubID, sysID) {
  return this.doctype(pubID, sysID);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.e"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>e (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.e)
- description and source-code
```javascript
e = function (name, attributes, text) {
  return this.element(name, attributes, text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.ele"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>ele (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.ele)
- description and source-code
```javascript
ele = function (name, attributes, text) {
  return this.element(name, attributes, text);
}
```
- example usage
```shell
...
'''

### Usage:

''' js
var builder = require('xmlbuilder');
var xml = builder.create('root')
  .ele('xmlbuilder')
    .ele('repo', {'type': 'git'}, 'git://github.com/oozcitak/xmlbuilder-js.git')
  .end({ pretty: true});

console.log(xml);
'''

will result in:
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.element"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>element (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.element)
- description and source-code
```javascript
element = function (name, attributes, text) {
  var childNode, item, j, k, key, lastChild, len, len1, ref1, val;
  lastChild = null;
  if (attributes == null) {
    attributes = {};
  }
  attributes = attributes.valueOf();
  if (!isObject(attributes)) {
    ref1 = [attributes, text], text = ref1[0], attributes = ref1[1];
  }
  if (name != null) {
    name = name.valueOf();
  }
  if (Array.isArray(name)) {
    for (j = 0, len = name.length; j < len; j++) {
      item = name[j];
      lastChild = this.element(item);
    }
  } else if (isFunction(name)) {
    lastChild = this.element(name.apply());
  } else if (isObject(name)) {
    for (key in name) {
      if (!hasProp.call(name, key)) continue;
      val = name[key];
      if (isFunction(val)) {
        val = val.apply();
      }
      if ((isObject(val)) && (isEmpty(val))) {
        val = null;
      }
      if (!this.options.ignoreDecorators && this.stringify.convertAttKey && key.indexOf(this.stringify.convertAttKey) === 0) {
        lastChild = this.attribute(key.substr(this.stringify.convertAttKey.length), val);
      } else if (!this.options.separateArrayItems && Array.isArray(val)) {
        for (k = 0, len1 = val.length; k < len1; k++) {
          item = val[k];
          childNode = {};
          childNode[key] = item;
          lastChild = this.element(childNode);
        }
      } else if (isObject(val)) {
        lastChild = this.element(key);
        lastChild.element(val);
      } else {
        lastChild = this.element(key, val);
      }
    }
  } else {
    if (!this.options.ignoreDecorators && this.stringify.convertTextKey && name.indexOf(this.stringify.convertTextKey) === 0) {
      lastChild = this.text(text);
    } else if (!this.options.ignoreDecorators && this.stringify.convertCDataKey && name.indexOf(this.stringify.convertCDataKey) ===
0) {
      lastChild = this.cdata(text);
    } else if (!this.options.ignoreDecorators && this.stringify.convertCommentKey && name.indexOf(this.stringify.convertCommentKey
) === 0) {
      lastChild = this.comment(text);
    } else if (!this.options.ignoreDecorators && this.stringify.convertRawKey && name.indexOf(this.stringify.convertRawKey) ===
0) {
      lastChild = this.raw(text);
    } else if (!this.options.ignoreDecorators && this.stringify.convertPIKey && name.indexOf(this.stringify.convertPIKey) === 0) {
      lastChild = this.instruction(name.substr(this.stringify.convertPIKey.length), text);
    } else {
      lastChild = this.node(name, attributes, text);
    }
  }
  if (lastChild == null) {
    throw new Error("Could not create any elements with: " + name);
  }
  return lastChild;
}
```
- example usage
```shell
...
};

XMLDocType.prototype.toString = function(options) {
  return this.options.writer.set(options).docType(this);
};

XMLDocType.prototype.ele = function(name, value) {
  return this.element(name, value);
};

XMLDocType.prototype.att = function(elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  return this.attList(elementName, attributeName, attributeType, defaultValueType, defaultValue);
};

XMLDocType.prototype.ent = function(name, value) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.end"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>end (options)](#apidoc.element.xmlbuilder.XMLNode.prototype.end)
- description and source-code
```javascript
end = function (options) {
  return this.document().end(options);
}
```
- example usage
```shell
...
### Usage:

''' js
var builder = require('xmlbuilder');
var xml = builder.create('root')
  .ele('xmlbuilder')
    .ele('repo', {'type': 'git'}, 'git://github.com/oozcitak/xmlbuilder-js.git')
  .end({ pretty: true});

console.log(xml);
'''

will result in:

''' xml
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.i"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>i (target, value)](#apidoc.element.xmlbuilder.XMLNode.prototype.i)
- description and source-code
```javascript
i = function (target, value) {
  return this.instruction(target, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.importDocument"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>importDocument (doc)](#apidoc.element.xmlbuilder.XMLNode.prototype.importDocument)
- description and source-code
```javascript
importDocument = function (doc) {
  var clonedRoot;
  clonedRoot = doc.root().clone();
  clonedRoot.parent = this;
  clonedRoot.isRoot = false;
  this.children.push(clonedRoot);
  return this;
}
```
- example usage
```shell
...
    };

    XMLNode.prototype.u = function() {
      return this.up();
    };

    XMLNode.prototype.importXMLBuilder = function(doc) {
      return this.importDocument(doc);
    };

    return XMLNode;

  })();

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.importXMLBuilder"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>importXMLBuilder (doc)](#apidoc.element.xmlbuilder.XMLNode.prototype.importXMLBuilder)
- description and source-code
```javascript
importXMLBuilder = function (doc) {
  return this.importDocument(doc);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.ins"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>ins (target, value)](#apidoc.element.xmlbuilder.XMLNode.prototype.ins)
- description and source-code
```javascript
ins = function (target, value) {
  return this.instruction(target, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.insertAfter"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>insertAfter (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.insertAfter)
- description and source-code
```javascript
insertAfter = function (name, attributes, text) {
  var child, i, removed;
  if (this.isRoot) {
    throw new Error("Cannot insert elements at root level");
  }
  i = this.parent.children.indexOf(this);
  removed = this.parent.children.splice(i + 1);
  child = this.parent.element(name, attributes, text);
  Array.prototype.push.apply(this.parent.children, removed);
  return child;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.insertBefore"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>insertBefore (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.insertBefore)
- description and source-code
```javascript
insertBefore = function (name, attributes, text) {
  var child, i, removed;
  if (this.isRoot) {
    throw new Error("Cannot insert elements at root level");
  }
  i = this.parent.children.indexOf(this);
  removed = this.parent.children.splice(i);
  child = this.parent.element(name, attributes, text);
  Array.prototype.push.apply(this.parent.children, removed);
  return child;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.instruction"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>instruction (target, value)](#apidoc.element.xmlbuilder.XMLNode.prototype.instruction)
- description and source-code
```javascript
instruction = function (target, value) {
  var insTarget, insValue, instruction, j, len;
  if (target != null) {
    target = target.valueOf();
  }
  if (value != null) {
    value = value.valueOf();
  }
  if (Array.isArray(target)) {
    for (j = 0, len = target.length; j < len; j++) {
      insTarget = target[j];
      this.instruction(insTarget);
    }
  } else if (isObject(target)) {
    for (insTarget in target) {
      if (!hasProp.call(target, insTarget)) continue;
      insValue = target[insTarget];
      this.instruction(insTarget, insValue);
    }
  } else {
    if (isFunction(value)) {
      value = value.apply();
    }
    instruction = new XMLProcessingInstruction(this, target, value);
    this.children.push(instruction);
  }
  return this;
}
```
- example usage
```shell
...
}
if (value != null) {
  value = value.valueOf();
}
if (Array.isArray(target)) {
  for (i = 0, len = target.length; i < len; i++) {
    insTarget = target[i];
    this.instruction(insTarget);
  }
} else if (isObject(target)) {
  for (insTarget in target) {
    if (!hasProp.call(target, insTarget)) continue;
    insValue = target[insTarget];
    this.instruction(insTarget, insValue);
  }
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.instructionAfter"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>instructionAfter (target, value)](#apidoc.element.xmlbuilder.XMLNode.prototype.instructionAfter)
- description and source-code
```javascript
instructionAfter = function (target, value) {
  var child, i, removed;
  i = this.parent.children.indexOf(this);
  removed = this.parent.children.splice(i + 1);
  child = this.parent.instruction(target, value);
  Array.prototype.push.apply(this.parent.children, removed);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.instructionBefore"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>instructionBefore (target, value)](#apidoc.element.xmlbuilder.XMLNode.prototype.instructionBefore)
- description and source-code
```javascript
instructionBefore = function (target, value) {
  var child, i, removed;
  i = this.parent.children.indexOf(this);
  removed = this.parent.children.splice(i);
  child = this.parent.instruction(target, value);
  Array.prototype.push.apply(this.parent.children, removed);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.n"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>n (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.n)
- description and source-code
```javascript
n = function (name, attributes, text) {
  return this.node(name, attributes, text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.next"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>next ()](#apidoc.element.xmlbuilder.XMLNode.prototype.next)
- description and source-code
```javascript
next = function () {
  var i;
  i = this.parent.children.indexOf(this);
  if (i === -1 || i === this.parent.children.length - 1) {
    throw new Error("Already at the last node");
  }
  return this.parent.children[i + 1];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.nod"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>nod (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.nod)
- description and source-code
```javascript
nod = function (name, attributes, text) {
  return this.node(name, attributes, text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.node"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>node (name, attributes, text)](#apidoc.element.xmlbuilder.XMLNode.prototype.node)
- description and source-code
```javascript
node = function (name, attributes, text) {
  var child, ref1;
  if (name != null) {
    name = name.valueOf();
  }
  attributes || (attributes = {});
  attributes = attributes.valueOf();
  if (!isObject(attributes)) {
    ref1 = [attributes, text], text = ref1[0], attributes = ref1[1];
  }
  child = new XMLElement(this, name, attributes);
  if (text != null) {
    child.text(text);
  }
  this.children.push(child);
  return child;
}
```
- example usage
```shell
...
  return this;
};

XMLDocumentCB.prototype.element = function(name, attributes, text) {
  if (this.currentNode && this.currentNode instanceof XMLDocType) {
    return this.dtdElement.apply(this, arguments);
  } else {
    return this.node(name, attributes, text);
  }
};

XMLDocumentCB.prototype.attribute = function(name, value) {
  var attName, attValue;
  if (!this.currentNode || this.currentNode.children) {
    throw new Error("att() can only be used immediately after an ele() call in callback mode");
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.prev"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>prev ()](#apidoc.element.xmlbuilder.XMLNode.prototype.prev)
- description and source-code
```javascript
prev = function () {
  var i;
  i = this.parent.children.indexOf(this);
  if (i < 1) {
    throw new Error("Already at the first node");
  }
  return this.parent.children[i - 1];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.r"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>r (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.r)
- description and source-code
```javascript
r = function (value) {
  return this.raw(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.raw"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>raw (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.raw)
- description and source-code
```javascript
raw = function (value) {
  var child;
  child = new XMLRaw(this, value);
  this.children.push(child);
  return this;
}
```
- example usage
```shell
...
  return this;
};

XMLDocumentCB.prototype.raw = function(value) {
  var node;
  this.openCurrent();
  node = new XMLRaw(this, value);
  this.onData(this.writer.raw(node, this.currentLevel + 1));
  return this;
};

XMLDocumentCB.prototype.instruction = function(target, value) {
  var i, insTarget, insValue, len, node;
  this.openCurrent();
  if (target != null) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.remove"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>remove ()](#apidoc.element.xmlbuilder.XMLNode.prototype.remove)
- description and source-code
```javascript
remove = function () {
  var i, ref1;
  if (this.isRoot) {
    throw new Error("Cannot remove the root element");
  }
  i = this.parent.children.indexOf(this);
  [].splice.apply(this.parent.children, [i, i - i + 1].concat(ref1 = [])), ref1;
  return this.parent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.root"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>root ()](#apidoc.element.xmlbuilder.XMLNode.prototype.root)
- description and source-code
```javascript
root = function () {
  var node;
  node = this;
  while (node) {
    if (node.isDocument) {
      return node.rootObject;
    } else if (node.isRoot) {
      return node;
    } else {
      node = node.parent;
    }
  }
}
```
- example usage
```shell
...
    };

    XMLDocType.prototype.not = function(name, value) {
      return this.notation(name, value);
    };

    XMLDocType.prototype.up = function() {
      return this.root() || this.documentObject;
    };

    return XMLDocType;

  })(XMLNode);

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.t"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>t (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.t)
- description and source-code
```javascript
t = function (value) {
  return this.text(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.text"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>text (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.text)
- description and source-code
```javascript
text = function (value) {
  var child;
  child = new XMLText(this, value);
  this.children.push(child);
  return this;
}
```
- example usage
```shell
...
    ref1 = [attributes, text], text = ref1[0], attributes = ref1[1];
  }
  this.currentNode = new XMLElement(this, name, attributes);
  this.currentNode.children = false;
  this.currentLevel++;
  this.openTags[this.currentLevel] = this.currentNode;
  if (text != null) {
    this.text(text);
  }
  return this;
};

XMLDocumentCB.prototype.element = function(name, attributes, text) {
  if (this.currentNode && this.currentNode instanceof XMLDocType) {
    return this.dtdElement.apply(this, arguments);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.txt"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>txt (value)](#apidoc.element.xmlbuilder.XMLNode.prototype.txt)
- description and source-code
```javascript
txt = function (value) {
  return this.text(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.u"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>u ()](#apidoc.element.xmlbuilder.XMLNode.prototype.u)
- description and source-code
```javascript
u = function () {
  return this.up();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLNode.prototype.up"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLNode.prototype.</span>up ()](#apidoc.element.xmlbuilder.XMLNode.prototype.up)
- description and source-code
```javascript
up = function () {
  if (this.isRoot) {
    throw new Error("The root node has no parent. Use doc() if you need to get the document object.");
  }
  return this.parent;
}
```
- example usage
```shell
...
  delete this.openTags[this.currentLevel];
  this.currentLevel--;
  return this;
};

XMLDocumentCB.prototype.end = function() {
  while (this.currentLevel >= 0) {
    this.up();
  }
  return this.onEnd();
};

XMLDocumentCB.prototype.openCurrent = function() {
  if (this.currentNode) {
    this.currentNode.children = true;
...
```



# <a name="apidoc.module.xmlbuilder.XMLProcessingInstruction"></a>[module xmlbuilder.XMLProcessingInstruction](#apidoc.module.xmlbuilder.XMLProcessingInstruction)

#### <a name="apidoc.element.xmlbuilder.XMLProcessingInstruction.XMLProcessingInstruction"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLProcessingInstruction (parent, target, value)](#apidoc.element.xmlbuilder.XMLProcessingInstruction.XMLProcessingInstruction)
- description and source-code
```javascript
function XMLProcessingInstruction(parent, target, value) {
  XMLProcessingInstruction.__super__.constructor.call(this, parent);
  if (target == null) {
    throw new Error("Missing instruction target");
  }
  this.target = this.stringify.insTarget(target);
  if (value) {
    this.value = this.stringify.insValue(value);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLProcessingInstruction.prototype"></a>[module xmlbuilder.XMLProcessingInstruction.prototype](#apidoc.module.xmlbuilder.XMLProcessingInstruction.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLProcessingInstruction.prototype.clone"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLProcessingInstruction.prototype.</span>clone ()](#apidoc.element.xmlbuilder.XMLProcessingInstruction.prototype.clone)
- description and source-code
```javascript
clone = function () {
  return Object.create(this);
}
```
- example usage
```shell
...
  clonedSelf.documentObject = null;
}
clonedSelf.attributes = {};
ref1 = this.attributes;
for (attName in ref1) {
  if (!hasProp.call(ref1, attName)) continue;
  att = ref1[attName];
  clonedSelf.attributes[attName] = att.clone();
}
clonedSelf.children = [];
this.children.forEach(function(child) {
  var clonedChild;
  clonedChild = child.clone();
  clonedChild.parent = clonedSelf;
  return clonedSelf.children.push(clonedChild);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLProcessingInstruction.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLProcessingInstruction.prototype.</span>constructor (parent, target, value)](#apidoc.element.xmlbuilder.XMLProcessingInstruction.prototype.constructor)
- description and source-code
```javascript
function XMLProcessingInstruction(parent, target, value) {
  XMLProcessingInstruction.__super__.constructor.call(this, parent);
  if (target == null) {
    throw new Error("Missing instruction target");
  }
  this.target = this.stringify.insTarget(target);
  if (value) {
    this.value = this.stringify.insValue(value);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLProcessingInstruction.prototype.toString"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLProcessingInstruction.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLProcessingInstruction.prototype.toString)
- description and source-code
```javascript
toString = function (options) {
  return this.options.writer.set(options).processingInstruction(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLRaw"></a>[module xmlbuilder.XMLRaw](#apidoc.module.xmlbuilder.XMLRaw)

#### <a name="apidoc.element.xmlbuilder.XMLRaw.XMLRaw"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLRaw (parent, text)](#apidoc.element.xmlbuilder.XMLRaw.XMLRaw)
- description and source-code
```javascript
function XMLRaw(parent, text) {
  XMLRaw.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing raw text");
  }
  this.value = this.stringify.raw(text);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLRaw.prototype"></a>[module xmlbuilder.XMLRaw.prototype](#apidoc.module.xmlbuilder.XMLRaw.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLRaw.prototype.clone"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLRaw.prototype.</span>clone ()](#apidoc.element.xmlbuilder.XMLRaw.prototype.clone)
- description and source-code
```javascript
clone = function () {
  return Object.create(this);
}
```
- example usage
```shell
...
  clonedSelf.documentObject = null;
}
clonedSelf.attributes = {};
ref1 = this.attributes;
for (attName in ref1) {
  if (!hasProp.call(ref1, attName)) continue;
  att = ref1[attName];
  clonedSelf.attributes[attName] = att.clone();
}
clonedSelf.children = [];
this.children.forEach(function(child) {
  var clonedChild;
  clonedChild = child.clone();
  clonedChild.parent = clonedSelf;
  return clonedSelf.children.push(clonedChild);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLRaw.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLRaw.prototype.</span>constructor (parent, text)](#apidoc.element.xmlbuilder.XMLRaw.prototype.constructor)
- description and source-code
```javascript
function XMLRaw(parent, text) {
  XMLRaw.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing raw text");
  }
  this.value = this.stringify.raw(text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLRaw.prototype.toString"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLRaw.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLRaw.prototype.toString)
- description and source-code
```javascript
toString = function (options) {
  return this.options.writer.set(options).raw(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLStreamWriter"></a>[module xmlbuilder.XMLStreamWriter](#apidoc.module.xmlbuilder.XMLStreamWriter)

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.XMLStreamWriter"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStreamWriter (stream, options)](#apidoc.element.xmlbuilder.XMLStreamWriter.XMLStreamWriter)
- description and source-code
```javascript
function XMLStreamWriter(stream, options) {
  this.stream = stream;
  XMLStreamWriter.__super__.constructor.call(this, options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLStreamWriter.prototype"></a>[module xmlbuilder.XMLStreamWriter.prototype](#apidoc.module.xmlbuilder.XMLStreamWriter.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.attribute"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>attribute (att)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.attribute)
- description and source-code
```javascript
attribute = function (att) {
  return this.stream.write(' ' + att.name + '="' + att.value + '"');
}
```
- example usage
```shell
...
    }

    XMLAttribute.prototype.clone = function() {
      return Object.create(this);
    };

    XMLAttribute.prototype.toString = function(options) {
      return this.options.writer.set(options).attribute(this);
    };

    return XMLAttribute;

  })();

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.cdata"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>cdata (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.cdata)
- description and source-code
```javascript
cdata = function (node, level) {
  return this.stream.write(this.space(level) + '<![CDATA[' + node.text + ']]>' + this.endline(node));
}
```
- example usage
```shell
...
extend(XMLCData, superClass);

function XMLCData(parent, text) {
  XMLCData.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing CDATA text");
  }
  this.text = this.stringify.cdata(text);
}

XMLCData.prototype.clone = function() {
  return Object.create(this);
};

XMLCData.prototype.toString = function(options) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.comment"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>comment (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.comment)
- description and source-code
```javascript
comment = function (node, level) {
  return this.stream.write(this.space(level) + '<!-- ' + node.text + ' -->' + this.endline(node));
}
```
- example usage
```shell
...
extend(XMLComment, superClass);

function XMLComment(parent, text) {
  XMLComment.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing comment text");
  }
  this.text = this.stringify.comment(text);
}

XMLComment.prototype.clone = function() {
  return Object.create(this);
};

XMLComment.prototype.toString = function(options) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>constructor (stream, options)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.constructor)
- description and source-code
```javascript
function XMLStreamWriter(stream, options) {
  this.stream = stream;
  XMLStreamWriter.__super__.constructor.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.declaration"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>declaration (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.declaration)
- description and source-code
```javascript
declaration = function (node, level) {
  this.stream.write(this.space(level));
  this.stream.write('<?xml version="' + node.version + '"');
  if (node.encoding != null) {
    this.stream.write(' encoding="' + node.encoding + '"');
  }
  if (node.standalone != null) {
    this.stream.write(' standalone="' + node.standalone + '"');
  }
  this.stream.write('?>');
  return this.stream.write(this.endline(node));
}
```
- example usage
```shell
...
      }
      if (standalone != null) {
        this.standalone = this.stringify.xmlStandalone(standalone);
      }
    }

    XMLDeclaration.prototype.toString = function(options) {
      return this.options.writer.set(options).declaration(this);
    };

    return XMLDeclaration;

  })(XMLNode);

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.docType"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>docType (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.docType)
- description and source-code
```javascript
docType = function (node, level) {
  var child, i, len, ref;
  level || (level = 0);
  this.stream.write(this.space(level));
  this.stream.write('<!DOCTYPE ' + node.root().name);
  if (node.pubID && node.sysID) {
    this.stream.write(' PUBLIC "' + node.pubID + '" "' + node.sysID + '"');
  } else if (node.sysID) {
    this.stream.write(' SYSTEM "' + node.sysID + '"');
  }
  if (node.children.length > 0) {
    this.stream.write(' [');
    this.stream.write(this.endline(node));
    ref = node.children;
    for (i = 0, len = ref.length; i < len; i++) {
      child = ref[i];
      switch (false) {
        case !(child instanceof XMLDTDAttList):
          this.dtdAttList(child, level + 1);
          break;
        case !(child instanceof XMLDTDElement):
          this.dtdElement(child, level + 1);
          break;
        case !(child instanceof XMLDTDEntity):
          this.dtdEntity(child, level + 1);
          break;
        case !(child instanceof XMLDTDNotation):
          this.dtdNotation(child, level + 1);
          break;
        case !(child instanceof XMLCData):
          this.cdata(child, level + 1);
          break;
        case !(child instanceof XMLComment):
          this.comment(child, level + 1);
          break;
        case !(child instanceof XMLProcessingInstruction):
          this.processingInstruction(child, level + 1);
          break;
        default:
          throw new Error("Unknown DTD node type: " + child.constructor.name);
      }
    }
    this.stream.write(']');
  }
  this.stream.write('>');
  return this.stream.write(this.endline(node));
}
```
- example usage
```shell
...
  var child;
  child = new XMLDTDNotation(this, name, value);
  this.children.push(child);
  return this;
};

XMLDocType.prototype.toString = function(options) {
  return this.options.writer.set(options).docType(this);
};

XMLDocType.prototype.ele = function(name, value) {
  return this.element(name, value);
};

XMLDocType.prototype.att = function(elementName, attributeName, attributeType, defaultValueType, defaultValue) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.document"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>document (doc)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.document)
- description and source-code
```javascript
document = function (doc) {
  var child, i, j, len, len1, ref, ref1, results;
  ref = doc.children;
  for (i = 0, len = ref.length; i < len; i++) {
    child = ref[i];
    child.isLastRootNode = false;
  }
  doc.children[doc.children.length - 1].isLastRootNode = true;
  ref1 = doc.children;
  results = [];
  for (j = 0, len1 = ref1.length; j < len1; j++) {
    child = ref1[j];
    switch (false) {
      case !(child instanceof XMLDeclaration):
        results.push(this.declaration(child));
        break;
      case !(child instanceof XMLDocType):
        results.push(this.docType(child));
        break;
      case !(child instanceof XMLComment):
        results.push(this.comment(child));
        break;
      case !(child instanceof XMLProcessingInstruction):
        results.push(this.processingInstruction(child));
        break;
      default:
        results.push(this.element(child));
    }
  }
  return results;
}
```
- example usage
```shell
...
  var writerOptions;
  if (!writer) {
    writer = this.options.writer;
  } else if (isPlainObject(writer)) {
    writerOptions = writer;
    writer = this.options.writer.set(writerOptions);
  }
  return writer.document(this);
};

XMLDocument.prototype.toString = function(options) {
  return this.options.writer.set(options).document(this);
};

return XMLDocument;
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.dtdAttList"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>dtdAttList (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.dtdAttList)
- description and source-code
```javascript
dtdAttList = function (node, level) {
  this.stream.write(this.space(level) + '<!ATTLIST ' + node.elementName + ' ' + node.attributeName + ' ' + node.attributeType);
  if (node.defaultValueType !== '#DEFAULT') {
    this.stream.write(' ' + node.defaultValueType);
  }
  if (node.defaultValue) {
    this.stream.write(' "' + node.defaultValue + '"');
  }
  return this.stream.write('>' + this.endline(node));
}
```
- example usage
```shell
...
      this.attributeName = this.stringify.attName(attributeName);
      this.attributeType = this.stringify.dtdAttType(attributeType);
      this.defaultValue = this.stringify.dtdAttDefault(defaultValue);
      this.defaultValueType = defaultValueType;
    }

    XMLDTDAttList.prototype.toString = function(options) {
      return this.options.writer.set(options).dtdAttList(this);
    };

    return XMLDTDAttList;

  })(XMLNode);

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.dtdElement"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>dtdElement (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.dtdElement)
- description and source-code
```javascript
dtdElement = function (node, level) {
  return this.stream.write(this.space(level) + '<!ELEMENT ' + node.name + ' ' + node.value + '>' + this.endline(node));
}
```
- example usage
```shell
...
        value = '(' + value.join(',') + ')';
      }
      this.name = this.stringify.eleName(name);
      this.value = this.stringify.dtdElementValue(value);
    }

    XMLDTDElement.prototype.toString = function(options) {
      return this.options.writer.set(options).dtdElement(this);
    };

    return XMLDTDElement;

  })(XMLNode);

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.dtdEntity"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>dtdEntity (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.dtdEntity)
- description and source-code
```javascript
dtdEntity = function (node, level) {
  this.stream.write(this.space(level) + '<!ENTITY');
  if (node.pe) {
    this.stream.write(' %');
  }
  this.stream.write(' ' + node.name);
  if (node.value) {
    this.stream.write(' "' + node.value + '"');
  } else {
    if (node.pubID && node.sysID) {
      this.stream.write(' PUBLIC "' + node.pubID + '" "' + node.sysID + '"');
    } else if (node.sysID) {
      this.stream.write(' SYSTEM "' + node.sysID + '"');
    }
    if (node.nData) {
      this.stream.write(' NDATA ' + node.nData);
    }
  }
  return this.stream.write('>' + this.endline(node));
}
```
- example usage
```shell
...
        if (this.pe && this.nData) {
          throw new Error("Notation declaration is not allowed in a parameter entity");
        }
      }
    }

    XMLDTDEntity.prototype.toString = function(options) {
      return this.options.writer.set(options).dtdEntity(this);
    };

    return XMLDTDEntity;

  })(XMLNode);

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.dtdNotation"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>dtdNotation (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.dtdNotation)
- description and source-code
```javascript
dtdNotation = function (node, level) {
  this.stream.write(this.space(level) + '<!NOTATION ' + node.name);
  if (node.pubID && node.sysID) {
    this.stream.write(' PUBLIC "' + node.pubID + '" "' + node.sysID + '"');
  } else if (node.pubID) {
    this.stream.write(' PUBLIC "' + node.pubID + '"');
  } else if (node.sysID) {
    this.stream.write(' SYSTEM "' + node.sysID + '"');
  }
  return this.stream.write('>' + this.endline(node));
}
```
- example usage
```shell
...
      }
      if (value.sysID != null) {
        this.sysID = this.stringify.dtdSysID(value.sysID);
      }
    }

    XMLDTDNotation.prototype.toString = function(options) {
      return this.options.writer.set(options).dtdNotation(this);
    };

    return XMLDTDNotation;

  })(XMLNode);

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.element"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>element (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.element)
- description and source-code
```javascript
element = function (node, level) {
  var att, child, i, len, name, ref, ref1, space;
  level || (level = 0);
  space = this.space(level);
  this.stream.write(space + '<' + node.name);
  ref = node.attributes;
  for (name in ref) {
    if (!hasProp.call(ref, name)) continue;
    att = ref[name];
    this.attribute(att);
  }
  if (node.children.length === 0 || node.children.every(function(e) {
    return e.value === '';
  })) {
    if (this.allowEmpty) {
      this.stream.write('></' + node.name + '>');
    } else {
      this.stream.write('/>');
    }
  } else if (this.pretty && node.children.length === 1 && (node.children[0].value != null)) {
    this.stream.write('>');
    this.stream.write(node.children[0].value);
    this.stream.write('</' + node.name + '>');
  } else {
    this.stream.write('>' + this.newline);
    ref1 = node.children;
    for (i = 0, len = ref1.length; i < len; i++) {
      child = ref1[i];
      switch (false) {
        case !(child instanceof XMLCData):
          this.cdata(child, level + 1);
          break;
        case !(child instanceof XMLComment):
          this.comment(child, level + 1);
          break;
        case !(child instanceof XMLElement):
          this.element(child, level + 1);
          break;
        case !(child instanceof XMLRaw):
          this.raw(child, level + 1);
          break;
        case !(child instanceof XMLText):
          this.text(child, level + 1);
          break;
        case !(child instanceof XMLProcessingInstruction):
          this.processingInstruction(child, level + 1);
          break;
        default:
          throw new Error("Unknown XML node type: " + child.constructor.name);
      }
    }
    this.stream.write(space + '</' + node.name + '>');
  }
  return this.stream.write(this.endline(node));
}
```
- example usage
```shell
...
};

XMLDocType.prototype.toString = function(options) {
  return this.options.writer.set(options).docType(this);
};

XMLDocType.prototype.ele = function(name, value) {
  return this.element(name, value);
};

XMLDocType.prototype.att = function(elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  return this.attList(elementName, attributeName, attributeType, defaultValueType, defaultValue);
};

XMLDocType.prototype.ent = function(name, value) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.endline"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>endline (node)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.endline)
- description and source-code
```javascript
endline = function (node) {
  if (!node.isLastRootNode) {
    return this.newline;
  } else {
    return '';
  }
}
```
- example usage
```shell
...
};

XMLStreamWriter.prototype.attribute = function(att) {
  return this.stream.write(' ' + att.name + '="' + att.value + '"');
};

XMLStreamWriter.prototype.cdata = function(node, level) {
  return this.stream.write(this.space(level) + '<![CDATA[' + node.text + ']]>' + this.endline(node));
};

XMLStreamWriter.prototype.comment = function(node, level) {
  return this.stream.write(this.space(level) + '<!-- ' + node.text + ' -->' + this.endline(node));
};

XMLStreamWriter.prototype.declaration = function(node, level) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.processingInstruction"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>processingInstruction (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.processingInstruction)
- description and source-code
```javascript
processingInstruction = function (node, level) {
  this.stream.write(this.space(level) + '<?' + node.target);
  if (node.value) {
    this.stream.write(' ' + node.value);
  }
  return this.stream.write('?>' + this.endline(node));
}
```
- example usage
```shell
...
      this.instruction(insTarget, insValue);
    }
  } else {
    if (isFunction(value)) {
      value = value.apply();
    }
    node = new XMLProcessingInstruction(this, target, value);
    this.onData(this.writer.processingInstruction(node, this.currentLevel + 1));
  }
  return this;
};

XMLDocumentCB.prototype.declaration = function(version, encoding, standalone) {
  var node;
  this.openCurrent();
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.raw"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>raw (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.raw)
- description and source-code
```javascript
raw = function (node, level) {
  return this.stream.write(this.space(level) + node.value + this.endline(node));
}
```
- example usage
```shell
...
  return this;
};

XMLDocumentCB.prototype.raw = function(value) {
  var node;
  this.openCurrent();
  node = new XMLRaw(this, value);
  this.onData(this.writer.raw(node, this.currentLevel + 1));
  return this;
};

XMLDocumentCB.prototype.instruction = function(target, value) {
  var i, insTarget, insValue, len, node;
  this.openCurrent();
  if (target != null) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStreamWriter.prototype.text"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStreamWriter.prototype.</span>text (node, level)](#apidoc.element.xmlbuilder.XMLStreamWriter.prototype.text)
- description and source-code
```javascript
text = function (node, level) {
  return this.stream.write(this.space(level) + node.value + this.endline(node));
}
```
- example usage
```shell
...
    ref1 = [attributes, text], text = ref1[0], attributes = ref1[1];
  }
  this.currentNode = new XMLElement(this, name, attributes);
  this.currentNode.children = false;
  this.currentLevel++;
  this.openTags[this.currentLevel] = this.currentNode;
  if (text != null) {
    this.text(text);
  }
  return this;
};

XMLDocumentCB.prototype.element = function(name, attributes, text) {
  if (this.currentNode && this.currentNode instanceof XMLDocType) {
    return this.dtdElement.apply(this, arguments);
...
```



# <a name="apidoc.module.xmlbuilder.XMLStringWriter"></a>[module xmlbuilder.XMLStringWriter](#apidoc.module.xmlbuilder.XMLStringWriter)

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.XMLStringWriter"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStringWriter (options)](#apidoc.element.xmlbuilder.XMLStringWriter.XMLStringWriter)
- description and source-code
```javascript
function XMLStringWriter(options) {
  XMLStringWriter.__super__.constructor.call(this, options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLStringWriter.prototype"></a>[module xmlbuilder.XMLStringWriter.prototype](#apidoc.module.xmlbuilder.XMLStringWriter.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.attribute"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>attribute (att)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.attribute)
- description and source-code
```javascript
attribute = function (att) {
  return ' ' + att.name + '="' + att.value + '"';
}
```
- example usage
```shell
...
    }

    XMLAttribute.prototype.clone = function() {
      return Object.create(this);
    };

    XMLAttribute.prototype.toString = function(options) {
      return this.options.writer.set(options).attribute(this);
    };

    return XMLAttribute;

  })();

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.cdata"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>cdata (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.cdata)
- description and source-code
```javascript
cdata = function (node, level) {
  return this.space(level) + '<![CDATA[' + node.text + ']]>' + this.newline;
}
```
- example usage
```shell
...
extend(XMLCData, superClass);

function XMLCData(parent, text) {
  XMLCData.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing CDATA text");
  }
  this.text = this.stringify.cdata(text);
}

XMLCData.prototype.clone = function() {
  return Object.create(this);
};

XMLCData.prototype.toString = function(options) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.closeNode"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>closeNode (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.closeNode)
- description and source-code
```javascript
closeNode = function (node, level) {
  level || (level = 0);
  switch (false) {
    case !(node instanceof XMLElement):
      return this.space(level) + '</' + node.name + '>' + this.newline;
    case !(node instanceof XMLDocType):
      return this.space(level) + ']>' + this.newline;
  }
}
```
- example usage
```shell
...

    XMLDocumentCB.prototype.up = function() {
if (this.currentLevel < 0) {
  throw new Error("The document node has no parent");
}
if (this.currentNode) {
  if (this.currentNode.children) {
    this.closeNode(this.currentNode);
  } else {
    this.openNode(this.currentNode);
  }
  this.currentNode = null;
} else {
  this.closeNode(this.openTags[this.currentLevel]);
}
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.comment"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>comment (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.comment)
- description and source-code
```javascript
comment = function (node, level) {
  return this.space(level) + '<!-- ' + node.text + ' -->' + this.newline;
}
```
- example usage
```shell
...
extend(XMLComment, superClass);

function XMLComment(parent, text) {
  XMLComment.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing comment text");
  }
  this.text = this.stringify.comment(text);
}

XMLComment.prototype.clone = function() {
  return Object.create(this);
};

XMLComment.prototype.toString = function(options) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>constructor (options)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.constructor)
- description and source-code
```javascript
function XMLStringWriter(options) {
  XMLStringWriter.__super__.constructor.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.declaration"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>declaration (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.declaration)
- description and source-code
```javascript
declaration = function (node, level) {
  var r;
  r = this.space(level);
  r += '<?xml version="' + node.version + '"';
  if (node.encoding != null) {
    r += ' encoding="' + node.encoding + '"';
  }
  if (node.standalone != null) {
    r += ' standalone="' + node.standalone + '"';
  }
  r += '?>';
  r += this.newline;
  return r;
}
```
- example usage
```shell
...
      }
      if (standalone != null) {
        this.standalone = this.stringify.xmlStandalone(standalone);
      }
    }

    XMLDeclaration.prototype.toString = function(options) {
      return this.options.writer.set(options).declaration(this);
    };

    return XMLDeclaration;

  })(XMLNode);

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.docType"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>docType (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.docType)
- description and source-code
```javascript
docType = function (node, level) {
  var child, i, len, r, ref;
  level || (level = 0);
  r = this.space(level);
  r += '<!DOCTYPE ' + node.root().name;
  if (node.pubID && node.sysID) {
    r += ' PUBLIC "' + node.pubID + '" "' + node.sysID + '"';
  } else if (node.sysID) {
    r += ' SYSTEM "' + node.sysID + '"';
  }
  if (node.children.length > 0) {
    r += ' [';
    r += this.newline;
    ref = node.children;
    for (i = 0, len = ref.length; i < len; i++) {
      child = ref[i];
      r += (function() {
        switch (false) {
          case !(child instanceof XMLDTDAttList):
            return this.dtdAttList(child, level + 1);
          case !(child instanceof XMLDTDElement):
            return this.dtdElement(child, level + 1);
          case !(child instanceof XMLDTDEntity):
            return this.dtdEntity(child, level + 1);
          case !(child instanceof XMLDTDNotation):
            return this.dtdNotation(child, level + 1);
          case !(child instanceof XMLCData):
            return this.cdata(child, level + 1);
          case !(child instanceof XMLComment):
            return this.comment(child, level + 1);
          case !(child instanceof XMLProcessingInstruction):
            return this.processingInstruction(child, level + 1);
          default:
            throw new Error("Unknown DTD node type: " + child.constructor.name);
        }
      }).call(this);
    }
    r += ']';
  }
  r += '>';
  r += this.newline;
  return r;
}
```
- example usage
```shell
...
  var child;
  child = new XMLDTDNotation(this, name, value);
  this.children.push(child);
  return this;
};

XMLDocType.prototype.toString = function(options) {
  return this.options.writer.set(options).docType(this);
};

XMLDocType.prototype.ele = function(name, value) {
  return this.element(name, value);
};

XMLDocType.prototype.att = function(elementName, attributeName, attributeType, defaultValueType, defaultValue) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.document"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>document (doc)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.document)
- description and source-code
```javascript
document = function (doc) {
  var child, i, len, r, ref;
  r = '';
  ref = doc.children;
  for (i = 0, len = ref.length; i < len; i++) {
    child = ref[i];
    r += (function() {
      switch (false) {
        case !(child instanceof XMLDeclaration):
          return this.declaration(child);
        case !(child instanceof XMLDocType):
          return this.docType(child);
        case !(child instanceof XMLComment):
          return this.comment(child);
        case !(child instanceof XMLProcessingInstruction):
          return this.processingInstruction(child);
        default:
          return this.element(child, 0);
      }
    }).call(this);
  }
  if (this.pretty && r.slice(-this.newline.length) === this.newline) {
    r = r.slice(0, -this.newline.length);
  }
  return r;
}
```
- example usage
```shell
...
  var writerOptions;
  if (!writer) {
    writer = this.options.writer;
  } else if (isPlainObject(writer)) {
    writerOptions = writer;
    writer = this.options.writer.set(writerOptions);
  }
  return writer.document(this);
};

XMLDocument.prototype.toString = function(options) {
  return this.options.writer.set(options).document(this);
};

return XMLDocument;
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.dtdAttList"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>dtdAttList (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.dtdAttList)
- description and source-code
```javascript
dtdAttList = function (node, level) {
  var r;
  r = this.space(level) + '<!ATTLIST ' + node.elementName + ' ' + node.attributeName + ' ' + node.attributeType;
  if (node.defaultValueType !== '#DEFAULT') {
    r += ' ' + node.defaultValueType;
  }
  if (node.defaultValue) {
    r += ' "' + node.defaultValue + '"';
  }
  r += '>' + this.newline;
  return r;
}
```
- example usage
```shell
...
      this.attributeName = this.stringify.attName(attributeName);
      this.attributeType = this.stringify.dtdAttType(attributeType);
      this.defaultValue = this.stringify.dtdAttDefault(defaultValue);
      this.defaultValueType = defaultValueType;
    }

    XMLDTDAttList.prototype.toString = function(options) {
      return this.options.writer.set(options).dtdAttList(this);
    };

    return XMLDTDAttList;

  })(XMLNode);

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.dtdElement"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>dtdElement (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.dtdElement)
- description and source-code
```javascript
dtdElement = function (node, level) {
  return this.space(level) + '<!ELEMENT ' + node.name + ' ' + node.value + '>' + this.newline;
}
```
- example usage
```shell
...
        value = '(' + value.join(',') + ')';
      }
      this.name = this.stringify.eleName(name);
      this.value = this.stringify.dtdElementValue(value);
    }

    XMLDTDElement.prototype.toString = function(options) {
      return this.options.writer.set(options).dtdElement(this);
    };

    return XMLDTDElement;

  })(XMLNode);

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.dtdEntity"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>dtdEntity (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.dtdEntity)
- description and source-code
```javascript
dtdEntity = function (node, level) {
  var r;
  r = this.space(level) + '<!ENTITY';
  if (node.pe) {
    r += ' %';
  }
  r += ' ' + node.name;
  if (node.value) {
    r += ' "' + node.value + '"';
  } else {
    if (node.pubID && node.sysID) {
      r += ' PUBLIC "' + node.pubID + '" "' + node.sysID + '"';
    } else if (node.sysID) {
      r += ' SYSTEM "' + node.sysID + '"';
    }
    if (node.nData) {
      r += ' NDATA ' + node.nData;
    }
  }
  r += '>' + this.newline;
  return r;
}
```
- example usage
```shell
...
        if (this.pe && this.nData) {
          throw new Error("Notation declaration is not allowed in a parameter entity");
        }
      }
    }

    XMLDTDEntity.prototype.toString = function(options) {
      return this.options.writer.set(options).dtdEntity(this);
    };

    return XMLDTDEntity;

  })(XMLNode);

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.dtdNotation"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>dtdNotation (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.dtdNotation)
- description and source-code
```javascript
dtdNotation = function (node, level) {
  var r;
  r = this.space(level) + '<!NOTATION ' + node.name;
  if (node.pubID && node.sysID) {
    r += ' PUBLIC "' + node.pubID + '" "' + node.sysID + '"';
  } else if (node.pubID) {
    r += ' PUBLIC "' + node.pubID + '"';
  } else if (node.sysID) {
    r += ' SYSTEM "' + node.sysID + '"';
  }
  r += '>' + this.newline;
  return r;
}
```
- example usage
```shell
...
      }
      if (value.sysID != null) {
        this.sysID = this.stringify.dtdSysID(value.sysID);
      }
    }

    XMLDTDNotation.prototype.toString = function(options) {
      return this.options.writer.set(options).dtdNotation(this);
    };

    return XMLDTDNotation;

  })(XMLNode);

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.element"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>element (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.element)
- description and source-code
```javascript
element = function (node, level) {
  var att, child, i, len, name, r, ref, ref1, space;
  level || (level = 0);
  space = this.space(level);
  r = '';
  r += space + '<' + node.name;
  ref = node.attributes;
  for (name in ref) {
    if (!hasProp.call(ref, name)) continue;
    att = ref[name];
    r += this.attribute(att);
  }
  if (node.children.length === 0 || node.children.every(function(e) {
    return e.value === '';
  })) {
    if (this.allowEmpty) {
      r += '></' + node.name + '>' + this.newline;
    } else {
      r += '/>' + this.newline;
    }
  } else if (this.pretty && node.children.length === 1 && (node.children[0].value != null)) {
    r += '>';
    r += node.children[0].value;
    r += '</' + node.name + '>' + this.newline;
  } else {
    r += '>' + this.newline;
    ref1 = node.children;
    for (i = 0, len = ref1.length; i < len; i++) {
      child = ref1[i];
      r += (function() {
        switch (false) {
          case !(child instanceof XMLCData):
            return this.cdata(child, level + 1);
          case !(child instanceof XMLComment):
            return this.comment(child, level + 1);
          case !(child instanceof XMLElement):
            return this.element(child, level + 1);
          case !(child instanceof XMLRaw):
            return this.raw(child, level + 1);
          case !(child instanceof XMLText):
            return this.text(child, level + 1);
          case !(child instanceof XMLProcessingInstruction):
            return this.processingInstruction(child, level + 1);
          default:
            throw new Error("Unknown XML node type: " + child.constructor.name);
        }
      }).call(this);
    }
    r += space + '</' + node.name + '>' + this.newline;
  }
  return r;
}
```
- example usage
```shell
...
};

XMLDocType.prototype.toString = function(options) {
  return this.options.writer.set(options).docType(this);
};

XMLDocType.prototype.ele = function(name, value) {
  return this.element(name, value);
};

XMLDocType.prototype.att = function(elementName, attributeName, attributeType, defaultValueType, defaultValue) {
  return this.attList(elementName, attributeName, attributeType, defaultValueType, defaultValue);
};

XMLDocType.prototype.ent = function(name, value) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.openNode"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>openNode (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.openNode)
- description and source-code
```javascript
openNode = function (node, level) {
  var att, name, r, ref;
  level || (level = 0);
  if (node instanceof XMLElement) {
    r = this.space(level) + '<' + node.name;
    ref = node.attributes;
    for (name in ref) {
      if (!hasProp.call(ref, name)) continue;
      att = ref[name];
      r += this.attribute(att);
    }
    r += (node.children ? '>' : '/>') + this.newline;
    return r;
  } else {
    r = this.space(level) + '<!DOCTYPE ' + node.rootNodeName;
    if (node.pubID && node.sysID) {
      r += ' PUBLIC "' + node.pubID + '" "' + node.sysID + '"';
    } else if (node.sysID) {
      r += ' SYSTEM "' + node.sysID + '"';
    }
    r += (node.children ? ' [' : '>') + this.newline;
    return r;
  }
}
```
- example usage
```shell
...
if (this.currentLevel < 0) {
  throw new Error("The document node has no parent");
}
if (this.currentNode) {
  if (this.currentNode.children) {
    this.closeNode(this.currentNode);
  } else {
    this.openNode(this.currentNode);
  }
  this.currentNode = null;
} else {
  this.closeNode(this.openTags[this.currentLevel]);
}
delete this.openTags[this.currentLevel];
this.currentLevel--;
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.processingInstruction"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>processingInstruction (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.processingInstruction)
- description and source-code
```javascript
processingInstruction = function (node, level) {
  var r;
  r = this.space(level) + '<?' + node.target;
  if (node.value) {
    r += ' ' + node.value;
  }
  r += '?>' + this.newline;
  return r;
}
```
- example usage
```shell
...
      this.instruction(insTarget, insValue);
    }
  } else {
    if (isFunction(value)) {
      value = value.apply();
    }
    node = new XMLProcessingInstruction(this, target, value);
    this.onData(this.writer.processingInstruction(node, this.currentLevel + 1));
  }
  return this;
};

XMLDocumentCB.prototype.declaration = function(version, encoding, standalone) {
  var node;
  this.openCurrent();
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.raw"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>raw (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.raw)
- description and source-code
```javascript
raw = function (node, level) {
  return this.space(level) + node.value + this.newline;
}
```
- example usage
```shell
...
  return this;
};

XMLDocumentCB.prototype.raw = function(value) {
  var node;
  this.openCurrent();
  node = new XMLRaw(this, value);
  this.onData(this.writer.raw(node, this.currentLevel + 1));
  return this;
};

XMLDocumentCB.prototype.instruction = function(target, value) {
  var i, insTarget, insValue, len, node;
  this.openCurrent();
  if (target != null) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringWriter.prototype.text"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringWriter.prototype.</span>text (node, level)](#apidoc.element.xmlbuilder.XMLStringWriter.prototype.text)
- description and source-code
```javascript
text = function (node, level) {
  return this.space(level) + node.value + this.newline;
}
```
- example usage
```shell
...
    ref1 = [attributes, text], text = ref1[0], attributes = ref1[1];
  }
  this.currentNode = new XMLElement(this, name, attributes);
  this.currentNode.children = false;
  this.currentLevel++;
  this.openTags[this.currentLevel] = this.currentNode;
  if (text != null) {
    this.text(text);
  }
  return this;
};

XMLDocumentCB.prototype.element = function(name, attributes, text) {
  if (this.currentNode && this.currentNode instanceof XMLDocType) {
    return this.dtdElement.apply(this, arguments);
...
```



# <a name="apidoc.module.xmlbuilder.XMLStringifier"></a>[module xmlbuilder.XMLStringifier](#apidoc.module.xmlbuilder.XMLStringifier)

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.XMLStringifier"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLStringifier (options)](#apidoc.element.xmlbuilder.XMLStringifier.XMLStringifier)
- description and source-code
```javascript
function XMLStringifier(options) {
  this.assertLegalChar = bind(this.assertLegalChar, this);
  var key, ref1, value;
  options || (options = {});
  this.allowSurrogateChars = options.allowSurrogateChars;
  this.noDoubleEncoding = options.noDoubleEncoding;
  this.textCase = options.textCase;
  ref1 = options.stringify || {};
  for (key in ref1) {
    if (!hasProp.call(ref1, key)) continue;
    value = ref1[key];
    this[key] = value;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLStringifier.prototype"></a>[module xmlbuilder.XMLStringifier.prototype](#apidoc.module.xmlbuilder.XMLStringifier.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.applyCase"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>applyCase (str)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.applyCase)
- description and source-code
```javascript
applyCase = function (str) {
  switch (this.textCase) {
    case "camel":
      return camelCase(str);
    case "title":
      return titleCase(str);
    case "kebab":
    case "lower":
      return kebabCase(str);
    case "snake":
      return snakeCase(str);
    case "upper":
      return kebabCase(str).toUpperCase();
    default:
      return str;
  }
}
```
- example usage
```shell
...
    value = ref1[key];
    this[key] = value;
  }
}

XMLStringifier.prototype.eleName = function(val) {
  val = '' + val || '';
  val = this.applyCase(val);
  return this.assertLegalChar(val);
};

XMLStringifier.prototype.eleText = function(val) {
  val = '' + val || '';
  return this.assertLegalChar(this.elEscape(val));
};
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.assertLegalChar"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>assertLegalChar (str)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.assertLegalChar)
- description and source-code
```javascript
assertLegalChar = function (str) {
  var chars, chr;
  if (this.allowSurrogateChars) {
    chars = /[\u0000-\u0008\u000B-\u000C\u000E-\u001F\uFFFE-\uFFFF]/;
  } else {
    chars = /[\u0000-\u0008\u000B-\u000C\u000E-\u001F\uD800-\uDFFF\uFFFE-\uFFFF]/;
  }
  chr = str.match(chars);
  if (chr) {
    throw new Error("Invalid character (" + chr + ") in string: " + str + " at index " + chr.index);
  }
  return str;
}
```
- example usage
```shell
...
    this[key] = value;
  }
}

XMLStringifier.prototype.eleName = function(val) {
  val = '' + val || '';
  val = this.applyCase(val);
  return this.assertLegalChar(val);
};

XMLStringifier.prototype.eleText = function(val) {
  val = '' + val || '';
  return this.assertLegalChar(this.elEscape(val));
};
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.attEscape"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>attEscape (str)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.attEscape)
- description and source-code
```javascript
attEscape = function (str) {
  var ampregex;
  ampregex = this.noDoubleEncoding ? /(?!&\S+;)&/g : /&/g;
  return str.replace(ampregex, '&amp;').replace(/</g, '&lt;').replace(/"/g, '&quot;').replace(/\t/g, '&#x9;').replace(/\n/g, '&#
xA;').replace(/\r/g, '&#xD;');
}
```
- example usage
```shell
...
XMLStringifier.prototype.attName = function(val) {
  val = '' + val || '';
  return val = this.applyCase(val);
};

XMLStringifier.prototype.attValue = function(val) {
  val = '' + val || '';
  return this.attEscape(val);
};

XMLStringifier.prototype.insTarget = function(val) {
  return '' + val || '';
};

XMLStringifier.prototype.insValue = function(val) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.attName"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>attName (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.attName)
- description and source-code
```javascript
attName = function (val) {
  val = '' + val || '';
  return val = this.applyCase(val);
}
```
- example usage
```shell
...
  this.stringify = parent.stringify;
  if (name == null) {
    throw new Error("Missing attribute name of element " + parent.name);
  }
  if (value == null) {
    throw new Error("Missing attribute value for attribute " + name + " of element " + parent.name);
  }
  this.name = this.stringify.attName(name);
  this.value = this.stringify.attValue(value);
}

XMLAttribute.prototype.clone = function() {
  return Object.create(this);
};
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.attValue"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>attValue (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.attValue)
- description and source-code
```javascript
attValue = function (val) {
  val = '' + val || '';
  return this.attEscape(val);
}
```
- example usage
```shell
...
  if (name == null) {
    throw new Error("Missing attribute name of element " + parent.name);
  }
  if (value == null) {
    throw new Error("Missing attribute value for attribute " + name + " of element " + parent.name);
  }
  this.name = this.stringify.attName(name);
  this.value = this.stringify.attValue(value);
}

XMLAttribute.prototype.clone = function() {
  return Object.create(this);
};

XMLAttribute.prototype.toString = function(options) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.cdata"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>cdata (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.cdata)
- description and source-code
```javascript
cdata = function (val) {
  val = '' + val || '';
  val = val.replace(']]>', ']]]]><![CDATA[>');
  return this.assertLegalChar(val);
}
```
- example usage
```shell
...
extend(XMLCData, superClass);

function XMLCData(parent, text) {
  XMLCData.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing CDATA text");
  }
  this.text = this.stringify.cdata(text);
}

XMLCData.prototype.clone = function() {
  return Object.create(this);
};

XMLCData.prototype.toString = function(options) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.comment"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>comment (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.comment)
- description and source-code
```javascript
comment = function (val) {
  val = '' + val || '';
  if (val.match(/--/)) {
    throw new Error("Comment text cannot contain double-hypen: " + val);
  }
  return this.assertLegalChar(val);
}
```
- example usage
```shell
...
extend(XMLComment, superClass);

function XMLComment(parent, text) {
  XMLComment.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing comment text");
  }
  this.text = this.stringify.comment(text);
}

XMLComment.prototype.clone = function() {
  return Object.create(this);
};

XMLComment.prototype.toString = function(options) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdAttDefault"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>dtdAttDefault (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdAttDefault)
- description and source-code
```javascript
dtdAttDefault = function (val) {
  if (val != null) {
    return '' + val || '';
  } else {
    return val;
  }
}
```
- example usage
```shell
...
  }
  if (defaultValue && !defaultValueType.match(/^(#FIXED|#DEFAULT)$/)) {
    throw new Error("Default value only applies to #FIXED or #DEFAULT");
  }
  this.elementName = this.stringify.eleName(elementName);
  this.attributeName = this.stringify.attName(attributeName);
  this.attributeType = this.stringify.dtdAttType(attributeType);
  this.defaultValue = this.stringify.dtdAttDefault(defaultValue);
  this.defaultValueType = defaultValueType;
}

XMLDTDAttList.prototype.toString = function(options) {
  return this.options.writer.set(options).dtdAttList(this);
};
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdAttType"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>dtdAttType (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdAttType)
- description and source-code
```javascript
dtdAttType = function (val) {
  return '' + val || '';
}
```
- example usage
```shell
...
    throw new Error("Invalid default value type; expected: #REQUIRED, #IMPLIED, #FIXED or #DEFAULT");
  }
  if (defaultValue && !defaultValueType.match(/^(#FIXED|#DEFAULT)$/)) {
    throw new Error("Default value only applies to #FIXED or #DEFAULT");
  }
  this.elementName = this.stringify.eleName(elementName);
  this.attributeName = this.stringify.attName(attributeName);
  this.attributeType = this.stringify.dtdAttType(attributeType);
  this.defaultValue = this.stringify.dtdAttDefault(defaultValue);
  this.defaultValueType = defaultValueType;
}

XMLDTDAttList.prototype.toString = function(options) {
  return this.options.writer.set(options).dtdAttList(this);
};
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdElementValue"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>dtdElementValue (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdElementValue)
- description and source-code
```javascript
dtdElementValue = function (val) {
  return '' + val || '';
}
```
- example usage
```shell
...
  if (!value) {
    value = '(#PCDATA)';
  }
  if (Array.isArray(value)) {
    value = '(' + value.join(',') + ')';
  }
  this.name = this.stringify.eleName(name);
  this.value = this.stringify.dtdElementValue(value);
}

XMLDTDElement.prototype.toString = function(options) {
  return this.options.writer.set(options).dtdElement(this);
};

return XMLDTDElement;
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdEntityValue"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>dtdEntityValue (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdEntityValue)
- description and source-code
```javascript
dtdEntityValue = function (val) {
  return '' + val || '';
}
```
- example usage
```shell
...
}
if (value == null) {
  throw new Error("Missing entity value");
}
this.pe = !!pe;
this.name = this.stringify.eleName(name);
if (!isObject(value)) {
  this.value = this.stringify.dtdEntityValue(value);
} else {
  if (!value.pubID && !value.sysID) {
    throw new Error("Public and/or system identifiers are required for an external entity");
  }
  if (value.pubID && !value.sysID) {
    throw new Error("System identifier is required for a public external entity");
  }
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdNData"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>dtdNData (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdNData)
- description and source-code
```javascript
dtdNData = function (val) {
  return '' + val || '';
}
```
- example usage
```shell
...
    if (value.pubID != null) {
      this.pubID = this.stringify.dtdPubID(value.pubID);
    }
    if (value.sysID != null) {
      this.sysID = this.stringify.dtdSysID(value.sysID);
    }
    if (value.nData != null) {
      this.nData = this.stringify.dtdNData(value.nData);
    }
    if (this.pe && this.nData) {
      throw new Error("Notation declaration is not allowed in a parameter entity");
    }
  }
}
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdPubID"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>dtdPubID (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdPubID)
- description and source-code
```javascript
dtdPubID = function (val) {
  return '' + val || '';
}
```
- example usage
```shell
...
if (!value.pubID && !value.sysID) {
  throw new Error("Public and/or system identifiers are required for an external entity");
}
if (value.pubID && !value.sysID) {
  throw new Error("System identifier is required for a public external entity");
}
if (value.pubID != null) {
  this.pubID = this.stringify.dtdPubID(value.pubID);
}
if (value.sysID != null) {
  this.sysID = this.stringify.dtdSysID(value.sysID);
}
if (value.nData != null) {
  this.nData = this.stringify.dtdNData(value.nData);
}
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdSysID"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>dtdSysID (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.dtdSysID)
- description and source-code
```javascript
dtdSysID = function (val) {
  return '' + val || '';
}
```
- example usage
```shell
...
if (value.pubID && !value.sysID) {
  throw new Error("System identifier is required for a public external entity");
}
if (value.pubID != null) {
  this.pubID = this.stringify.dtdPubID(value.pubID);
}
if (value.sysID != null) {
  this.sysID = this.stringify.dtdSysID(value.sysID);
}
if (value.nData != null) {
  this.nData = this.stringify.dtdNData(value.nData);
}
if (this.pe && this.nData) {
  throw new Error("Notation declaration is not allowed in a parameter entity");
}
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.elEscape"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>elEscape (str)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.elEscape)
- description and source-code
```javascript
elEscape = function (str) {
  var ampregex;
  ampregex = this.noDoubleEncoding ? /(?!&\S+;)&/g : /&/g;
  return str.replace(ampregex, '&amp;').replace(/</g, '&lt;').replace(/>/g, '&gt;').replace(/\r/g, '&#xD;');
}
```
- example usage
```shell
...
  val = '' + val || '';
  val = this.applyCase(val);
  return this.assertLegalChar(val);
};

XMLStringifier.prototype.eleText = function(val) {
  val = '' + val || '';
  return this.assertLegalChar(this.elEscape(val));
};

XMLStringifier.prototype.cdata = function(val) {
  val = '' + val || '';
  val = val.replace(']]>', ']]]]><![CDATA[>');
  return this.assertLegalChar(val);
};
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.eleName"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>eleName (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.eleName)
- description and source-code
```javascript
eleName = function (val) {
  val = '' + val || '';
  val = this.applyCase(val);
  return this.assertLegalChar(val);
}
```
- example usage
```shell
...
  }
  if (!defaultValueType.match(/^(#REQUIRED|#IMPLIED|#FIXED|#DEFAULT)$/)) {
    throw new Error("Invalid default value type; expected: #REQUIRED, #IMPLIED, #FIXED or #DEFAULT");
  }
  if (defaultValue && !defaultValueType.match(/^(#FIXED|#DEFAULT)$/)) {
    throw new Error("Default value only applies to #FIXED or #DEFAULT");
  }
  this.elementName = this.stringify.eleName(elementName);
  this.attributeName = this.stringify.attName(attributeName);
  this.attributeType = this.stringify.dtdAttType(attributeType);
  this.defaultValue = this.stringify.dtdAttDefault(defaultValue);
  this.defaultValueType = defaultValueType;
}

XMLDTDAttList.prototype.toString = function(options) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.eleText"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>eleText (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.eleText)
- description and source-code
```javascript
eleText = function (val) {
  val = '' + val || '';
  return this.assertLegalChar(this.elEscape(val));
}
```
- example usage
```shell
...
extend(XMLText, superClass);

function XMLText(parent, text) {
  XMLText.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing element text");
  }
  this.value = this.stringify.eleText(text);
}

XMLText.prototype.clone = function() {
  return Object.create(this);
};

XMLText.prototype.toString = function(options) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.insTarget"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>insTarget (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.insTarget)
- description and source-code
```javascript
insTarget = function (val) {
  return '' + val || '';
}
```
- example usage
```shell
...
extend(XMLProcessingInstruction, superClass);

function XMLProcessingInstruction(parent, target, value) {
  XMLProcessingInstruction.__super__.constructor.call(this, parent);
  if (target == null) {
    throw new Error("Missing instruction target");
  }
  this.target = this.stringify.insTarget(target);
  if (value) {
    this.value = this.stringify.insValue(value);
  }
}

XMLProcessingInstruction.prototype.clone = function() {
  return Object.create(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.insValue"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>insValue (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.insValue)
- description and source-code
```javascript
insValue = function (val) {
  val = '' + val || '';
  if (val.match(/\?>/)) {
    throw new Error("Invalid processing instruction value: " + val);
  }
  return val;
}
```
- example usage
```shell
...
function XMLProcessingInstruction(parent, target, value) {
  XMLProcessingInstruction.__super__.constructor.call(this, parent);
  if (target == null) {
    throw new Error("Missing instruction target");
  }
  this.target = this.stringify.insTarget(target);
  if (value) {
    this.value = this.stringify.insValue(value);
  }
}

XMLProcessingInstruction.prototype.clone = function() {
  return Object.create(this);
};
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.raw"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>raw (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.raw)
- description and source-code
```javascript
raw = function (val) {
  return '' + val || '';
}
```
- example usage
```shell
...
  return this;
};

XMLDocumentCB.prototype.raw = function(value) {
  var node;
  this.openCurrent();
  node = new XMLRaw(this, value);
  this.onData(this.writer.raw(node, this.currentLevel + 1));
  return this;
};

XMLDocumentCB.prototype.instruction = function(target, value) {
  var i, insTarget, insValue, len, node;
  this.openCurrent();
  if (target != null) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.xmlEncoding"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>xmlEncoding (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.xmlEncoding)
- description and source-code
```javascript
xmlEncoding = function (val) {
  val = '' + val || '';
  if (!val.match(/^[A-Za-z](?:[A-Za-z0-9._-]|-)*$/)) {
    throw new Error("Invalid encoding: " + val);
  }
  return val;
}
```
- example usage
```shell
...
    ref = version, version = ref.version, encoding = ref.encoding, standalone = ref.standalone;
  }
  if (!version) {
    version = '1.0';
  }
  this.version = this.stringify.xmlVersion(version);
  if (encoding != null) {
    this.encoding = this.stringify.xmlEncoding(encoding);
  }
  if (standalone != null) {
    this.standalone = this.stringify.xmlStandalone(standalone);
  }
}

XMLDeclaration.prototype.toString = function(options) {
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.xmlStandalone"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>xmlStandalone (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.xmlStandalone)
- description and source-code
```javascript
xmlStandalone = function (val) {
  if (val) {
    return "yes";
  } else {
    return "no";
  }
}
```
- example usage
```shell
...
    version = '1.0';
  }
  this.version = this.stringify.xmlVersion(version);
  if (encoding != null) {
    this.encoding = this.stringify.xmlEncoding(encoding);
  }
  if (standalone != null) {
    this.standalone = this.stringify.xmlStandalone(standalone);
  }
}

XMLDeclaration.prototype.toString = function(options) {
  return this.options.writer.set(options).declaration(this);
};
...
```

#### <a name="apidoc.element.xmlbuilder.XMLStringifier.prototype.xmlVersion"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLStringifier.prototype.</span>xmlVersion (val)](#apidoc.element.xmlbuilder.XMLStringifier.prototype.xmlVersion)
- description and source-code
```javascript
xmlVersion = function (val) {
  val = '' + val || '';
  if (!val.match(/1\.[0-9]+/)) {
    throw new Error("Invalid version number: " + val);
  }
  return val;
}
```
- example usage
```shell
...
  XMLDeclaration.__super__.constructor.call(this, parent);
  if (isObject(version)) {
    ref = version, version = ref.version, encoding = ref.encoding, standalone = ref.standalone;
  }
  if (!version) {
    version = '1.0';
  }
  this.version = this.stringify.xmlVersion(version);
  if (encoding != null) {
    this.encoding = this.stringify.xmlEncoding(encoding);
  }
  if (standalone != null) {
    this.standalone = this.stringify.xmlStandalone(standalone);
  }
}
...
```



# <a name="apidoc.module.xmlbuilder.XMLText"></a>[module xmlbuilder.XMLText](#apidoc.module.xmlbuilder.XMLText)

#### <a name="apidoc.element.xmlbuilder.XMLText.XMLText"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLText (parent, text)](#apidoc.element.xmlbuilder.XMLText.XMLText)
- description and source-code
```javascript
function XMLText(parent, text) {
  XMLText.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing element text");
  }
  this.value = this.stringify.eleText(text);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLText.prototype"></a>[module xmlbuilder.XMLText.prototype](#apidoc.module.xmlbuilder.XMLText.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLText.prototype.clone"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLText.prototype.</span>clone ()](#apidoc.element.xmlbuilder.XMLText.prototype.clone)
- description and source-code
```javascript
clone = function () {
  return Object.create(this);
}
```
- example usage
```shell
...
  clonedSelf.documentObject = null;
}
clonedSelf.attributes = {};
ref1 = this.attributes;
for (attName in ref1) {
  if (!hasProp.call(ref1, attName)) continue;
  att = ref1[attName];
  clonedSelf.attributes[attName] = att.clone();
}
clonedSelf.children = [];
this.children.forEach(function(child) {
  var clonedChild;
  clonedChild = child.clone();
  clonedChild.parent = clonedSelf;
  return clonedSelf.children.push(clonedChild);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLText.prototype.constructor"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLText.prototype.</span>constructor (parent, text)](#apidoc.element.xmlbuilder.XMLText.prototype.constructor)
- description and source-code
```javascript
function XMLText(parent, text) {
  XMLText.__super__.constructor.call(this, parent);
  if (text == null) {
    throw new Error("Missing element text");
  }
  this.value = this.stringify.eleText(text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xmlbuilder.XMLText.prototype.toString"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLText.prototype.</span>toString (options)](#apidoc.element.xmlbuilder.XMLText.prototype.toString)
- description and source-code
```javascript
toString = function (options) {
  return this.options.writer.set(options).text(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLWriterBase"></a>[module xmlbuilder.XMLWriterBase](#apidoc.module.xmlbuilder.XMLWriterBase)

#### <a name="apidoc.element.xmlbuilder.XMLWriterBase.XMLWriterBase"></a>[function <span class="apidocSignatureSpan">xmlbuilder.</span>XMLWriterBase (options)](#apidoc.element.xmlbuilder.XMLWriterBase.XMLWriterBase)
- description and source-code
```javascript
function XMLWriterBase(options) {
  var key, ref, ref1, ref2, ref3, ref4, value;
  options || (options = {});
  this.pretty = options.pretty || false;
  this.allowEmpty = (ref = options.allowEmpty) != null ? ref : false;
  if (this.pretty) {
    this.indent = (ref1 = options.indent) != null ? ref1 : '  ';
    this.newline = (ref2 = options.newline) != null ? ref2 : '\n';
    this.offset = (ref3 = options.offset) != null ? ref3 : 0;
  } else {
    this.indent = '';
    this.newline = '';
    this.offset = 0;
  }
  ref4 = options.writer || {};
  for (key in ref4) {
    if (!hasProp.call(ref4, key)) continue;
    value = ref4[key];
    this[key] = value;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xmlbuilder.XMLWriterBase.prototype"></a>[module xmlbuilder.XMLWriterBase.prototype](#apidoc.module.xmlbuilder.XMLWriterBase.prototype)

#### <a name="apidoc.element.xmlbuilder.XMLWriterBase.prototype.set"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLWriterBase.prototype.</span>set (options)](#apidoc.element.xmlbuilder.XMLWriterBase.prototype.set)
- description and source-code
```javascript
set = function (options) {
  var key, ref, value;
  options || (options = {});
  if ("pretty" in options) {
    this.pretty = options.pretty;
  }
  if ("allowEmpty" in options) {
    this.allowEmpty = options.allowEmpty;
  }
  if (this.pretty) {
    this.indent = "indent" in options ? options.indent : '  ';
    this.newline = "newline" in options ? options.newline : '\n';
    this.offset = "offset" in options ? options.offset : 0;
  } else {
    this.indent = '';
    this.newline = '';
    this.offset = 0;
  }
  ref = options.writer || {};
  for (key in ref) {
    if (!hasProp.call(ref, key)) continue;
    value = ref[key];
    this[key] = value;
  }
  return this;
}
```
- example usage
```shell
...
    }

    XMLAttribute.prototype.clone = function() {
      return Object.create(this);
    };

    XMLAttribute.prototype.toString = function(options) {
      return this.options.writer.set(options).attribute(this);
    };

    return XMLAttribute;

  })();

}).call(this);
...
```

#### <a name="apidoc.element.xmlbuilder.XMLWriterBase.prototype.space"></a>[function <span class="apidocSignatureSpan">xmlbuilder.XMLWriterBase.prototype.</span>space (level)](#apidoc.element.xmlbuilder.XMLWriterBase.prototype.space)
- description and source-code
```javascript
space = function (level) {
  if (this.pretty) {
    return new Array((level || 0) + this.offset + 1).join(this.indent);
  } else {
    return '';
  }
}
```
- example usage
```shell
...
};

XMLStreamWriter.prototype.attribute = function(att) {
  return this.stream.write(' ' + att.name + '="' + att.value + '"');
};

XMLStreamWriter.prototype.cdata = function(node, level) {
  return this.stream.write(this.space(level) + '<![CDATA[' + node.text + ']]>' + this.endline(node));
};

XMLStreamWriter.prototype.comment = function(node, level) {
  return this.stream.write(this.space(level) + '<!-- ' + node.text + ' -->' + this.endline(node));
};

XMLStreamWriter.prototype.declaration = function(node, level) {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
