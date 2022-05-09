## Installation
1. go version: 1.18.1
2. require\
    These library will automatically install when run below command\
	github.com/andybalholm/brotli v1.0.4\
	github.com/fatih/structs v1.1.0\
	github.com/go-sql-driver/mysql v1.6.0\
	github.com/gofiber/fiber/v2 v2.32.0\
	github.com/google/uuid v1.3.0 \
	github.com/jinzhu/inflection v1.0.0\
	github.com/jinzhu/now v1.1.4\
	github.com/klauspost/compress v1.15.0 \
	github.com/mitchellh/mapstructure v1.5.0 \
	github.com/valyala/bytebufferpool v1.0.0\
	github.com/valyala/fasthttp v1.35.0 \
	github.com/valyala/tcplisten v1.0.0 \
	golang.org/x/sys v0.0.0-20220227234510-4e6760a101f9 \
	gorm.io/driver/mysql v1.3.3 \
	gorm.io/gorm v1.23.4 \
3. app.env file

## How to run
1. In the source project directory run this command to get dependency library
```
go mod download
```
2. Go mod tidy cleans up unused dependencies or adds missing dependencies
```
go mod tidy
```
3. Make sure in your GOPATH has those install library. Something like this\
    I has $GOPATH locate in this path
```
vmd@vmd:echo $GOPATH
/home/vmd/go
ls $GOPATH/pkg/mod/github.com
'!burnt!sushi'   go-check        kataras        sergi
'!cloudy!kit'    go-playground   klauspost     'shurcoo!l'
'!joker'         go-sql-driver   kr             smartystreets
'!shopify'       go-stack        labstack       stretchr
 ajg             gofiber         leodido        ugorji
 andybalholm     golang          mattn          valyala
 aymerick        google          microcosm-cc   vmihailenco
 chris-ramon     gopherjs        mitchellh      xdg-go
 davecgh         gorilla         modern-go      xeipuuv
 dgrijalva       imkira          moul           yalp
 eknkc           iris-contrib    pkg            yosssi
 fatih           jinzhu          pmezard        youmark
 gavv            joho            russross       yudai
 gin-contrib     json-iterator   ryanuber
 gin-gonic       jtolds          schollz
```
4. Run Makefile command
```
make run
```
5. If you dont have "make" install you could run the following cmd. Step by step\
    Go will create executable file by run this cmd.
```
go build
```
6.  
    Then run the file created above with the `start` options. Your "app.env" file locate in root directory then run this cmd.
```
./go-backend-api start
```
