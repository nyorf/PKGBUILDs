V=20211022

PREFIX = /usr/local

install:
	install -dm755 $(DESTDIR)$(PREFIX)/share/pacman/keyrings/
	install -m0644 mikoshi.gpg $(DESTDIR)$(PREFIX)/share/pacman/keyrings/
	install -m0644 mikoshi-trusted $(DESTDIR)$(PREFIX)/share/pacman/keyrings/
	install -m0644 mikoshi-revoked $(DESTDIR)$(PREFIX)/share/pacman/keyrings/

uninstall:
	rm -f $(DESTDIR)$(PREFIX)/share/pacman/keyrings/mikoshi{.gpg,-trusted,-revoked}
	rmdir -p --ignore-fail-on-non-empty $(DESTDIR)$(PREFIX)/share/pacman/keyrings/

.PHONY: install uninstall
