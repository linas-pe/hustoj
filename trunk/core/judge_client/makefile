all: judge_client.cc judge_client.http
	g++ -Wall -c -I/usr/include/mariadb -DOJ_USE_MYSQL judge_client.cc
	g++ -Wall -o judge_client judge_client.o -L/usr/lib/aarch64-linux-gnu -lmariadbclient
judge_client.http:judge_client.cc 
	g++ -o judge_client.http -O2 judge_client.cc
clean:
	rm judge_client judge_client.http
