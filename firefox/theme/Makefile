# Copyright (C) 2024 Aoki Kenji
# This file is part of Aoki Kenji's Dotfiles.
#
# Aoki Kenji's Dotfiles is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by the Free
# Software Foundation, either version 3 of the License, or (at your option) any
# later version.
#
# Aoki Kenji's Dotfiles is distributed in the hope that it will be useful, but
# WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
# FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more
# details.
#
# You should have received a copy of the GNU General Public License along with
# Aoki Kenji's Dotfiles. If not, see <https://www.gnu.org/licenses/>.

build: sora@aokikenji.xpi

clean:
	rm --force sora@aokikenji.xpi

install: sora@aokikenji.xpi
	install -D --mode 644 sora@aokikenji.xpi \
		/usr/lib/firefox/browser/extensions/sora@aokikenji.xpi

sora@aokikenji.xpi: manifest.json
	zip $@ -X --filesync manifest.json

.PHONY: build clean install
