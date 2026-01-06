<xsl:stylesheet version="1.0"
xmlns:xsl="http://www.w3.org/1999/XSL/Transform">

<xsl:template match="/">
<html>
<head>
<title>Trainers</title>
</head>

<body>

<h2>Trainers Information</h2>

<table border="1">
<tr>
<th>Name</th>
<th>Email</th>
<th>Course</th>
</tr>

<xsl:for-each select="trainers/trainer">
<tr>
<td><xsl:value-of select="Name"/></td>
<td><xsl:value-of select="Email"/></td>
<td><xsl:value-of select="Course"/></td>
</tr>
</xsl:for-each>

</table>

</body>
</html>
</xsl:template>

</xsl:stylesheet>
