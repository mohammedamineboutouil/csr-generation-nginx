openssl genrsa -out example.com.key 4096

openssl req -new -sha256 -out example.com.csr -key example.com.key -config ssl.conf

openssl req -in example.com.csr -noout -text