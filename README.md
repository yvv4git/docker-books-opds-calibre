# OPDS server Calibre


## HOW TO

1. Create dir.  
```
mkdir books
```

2. Start Calibre server.
```
make docker_start
```

2. Fill dir with books.  
```
copy mybook.epub to books/
```

3. Work with server over web.  
```
Open in browser http://localhost:8080
```


5. Convert pdf to epub.  
```
cp myBook.pdf books/
docker exec -ti calibre /bin/bash
ebook-convert myBook.pdf myBook.epub
```