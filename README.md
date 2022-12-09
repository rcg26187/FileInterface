# FileInterface

## URI schemes

### smb

```http

smb://[<user>@]<host>[:<port>][/[<path>]][?<param1>=<value1>[;
<param2>=<value2>]]

smb://[<user>@]<workgroup>[:<port>][/]

smb://[[<domain>;]<username>[:<password>]@]<server>[:<port>][/[<share>[/[<path>]]][?[<param>=<value>[<param2>=<value2>[...]]]]][2]
```

example:

```http
smb://workgroup;user:password@server/share/folder/file.txt 
```

### sftp

```http
sftp://[<user>[;fingerprint=<host-key fingerprint>]@]<host>[:<port>]/<path>/<file>
```

### Amazon S3 bucket

```http
s3://mybucket/puppy.jpg
```

### http

### https

### nfs

### ftp

```http
ftp://[<user>@]<host>[:<port>]/<path>/<file>
```

### file

Addressing files on local or network file systems

```http
file://[host]/path
```

(RFC 3986) file:[//host]/path

Since this is usually used for local files the **host** from RFC 1738 is often empty leading to a starting triple /. RFC 3986 allows an absolute path with no host part.
