# DisplayingInvoiceLinesUsingTemplate


The same invoice lines, as it was in part 4, were displayed after a template is defined.

Nothing changed in xml file.
However, In xslt file, I defined a template with the below match name.
```<xsl:template match="Invoice/InvoiceLine">```

Then invoked it for all invoice lines I have.
```<xsl:for-each select="Invoice/InvoiceLine">
	<xsl:apply-templates select="."/>
</xsl:for-each>```


This defined template and its invoke are specified in comments of Part5-DisplayingInvoiceLinesUsingTemplate.xslt for clarity.


The html output is same with part 4, you can see the output in output.html.
 