## About ms-access

Microsoft Access, also known as Microsoft Office Access, is a database management system from Microsoft that combines the relational Microsoft Jet Database Engine with a graphical user interface and software-development tools.

[Microsoft Access](http://en.wikipedia.org/wiki/Microsoft_Access), also known as Microsoft Office Access, is a rapid application database development tool.

It commonly uses the Jet or ACE database engine, but is not limited to these.

It is a member of the [![](//i.stack.imgur.com/0kGsy.png)ms-office](http://stackoverflow.com/questions/tagged/ms-office "show questions tagged 'ms-office'") suite of applications, included in the Professional and higher editions or sold separately. The current version is Microsoft Access 2013.  
 Applications built with Microsoft Access can be distributed to end users with a free run-time version of the application that lets them view databases without needing the full installation of Access.

This tag is version-agnostic. If you have a question about using a specific version, please tag your question appropriately so others know what version you are using. Ex:

*   [ms-access-2013](http://stackoverflow.com/questions/tagged/ms-access-2013 "show questions tagged 'ms-access-2013'")
*   [ms-access-2010](http://stackoverflow.com/questions/tagged/ms-access-2010 "show questions tagged 'ms-access-2010'")
*   [ms-access-2007](http://stackoverflow.com/questions/tagged/ms-access-2007 "show questions tagged 'ms-access-2007'")
*   [ms-access-2003](http://stackoverflow.com/questions/tagged/ms-access-2003 "show questions tagged 'ms-access-2003'")
*   [ms-access-2000](http://stackoverflow.com/questions/tagged/ms-access-2000 "show questions tagged 'ms-access-2000'")

and [access-vba](http://stackoverflow.com/questions/tagged/access-vba "show questions tagged 'access-vba'") or [vba](http://stackoverflow.com/questions/tagged/vba "show questions tagged 'vba'") if your question involves VBA.

## Links

*   [Microsoft Access Website](http://office.microsoft.com/en-us/access/)
*   [Microsoft Access Templates](http://office.microsoft.com/en-us/templates/results.aspx?qu=access&av=zac)
*   [Northwind database](http://blogs.office.com/b/microsoft-access/archive/2010/07/19/northwind-2010-web-database-is-now-available.aspx)

## Common errors

### Reserved Words

One of the most common problems with MS Access SQL is the use of a [reserved word](http://office.microsoft.com/en-ie/access-help/sql-reserved-words-HP001032249.aspx) in a query or SQL string. It is often suggested that these words are bracketed, `[RESERVED WORD]`, as is required for field (column) names containing spaces or special characters. But rather than trying to figure out what is and is not a reserved word and bracketing only those, using the convention of prefixing all field names with the table name — or better yet, the alias — will prevent this problem from occurring. This will save problems in other cases, not just reserved words. For example:

     SELECT a.id, b.id, b.name 
     FROM tablea a
     INNER JOIN tableb b 

It also makes the SQL compatible with other databases.

### Connection Strings

The usual [connection string](http://connectionstrings.com) for MS Access *.accdb files, that is, files created in Access 2007 format, is:

    Provider=Microsoft.ACE.OLEDB.12.0;Data Source=C:\myFolder\myAccess2007file.accdb;

The ACE connection string is backwards-compatible and will open *.mdb files; however, for *.mdb files, you can also use:

    Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\myFolder\myAccess.mdb;

Jet is often installed by default on Windows systems, but ACE is not. [ACE is available in both 32-bit and 64-bit.](http://www.microsoft.com/en-ie/download/details.aspx?id=13255)