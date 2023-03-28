all: judged.cc judged.http judgehub
	g++ -Wall -c -DOJ_USE_MYSQL -I/usr/include/mariadb judged.cc
	g++ -Wall -o judged judged.o -L/usr/lib/aarch64-linux-gnu -lmariadbclient

judged.http: judged.cc
	g++ -Wall -o judged.http judged.cc

judgedhub: judgehub.cc
	g++ -Wall -o judgehub judgehub.cc

