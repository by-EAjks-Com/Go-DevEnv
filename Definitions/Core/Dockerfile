#   by-EAjks.Com Go Development Environments
#   Copyright (C) 2025-2025 Andrea and Eric DELAGE <Contact@by-EAjks.Com>
#
#   This program is free software: you can redistribute it and/or modify
#   it under the terms of the GNU General Public License as published by
#   the Free Software Foundation, either version 3 of the License, or
#   (at your option) any later version.
#
#   This program is distributed in the hope that it will be useful,
#   but WITHOUT ANY WARRANTY; without even the implied warranty of
#   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
#   GNU General Public License for more details.
#
#   You should have received a copy of the GNU General Public License
#   along with this program.  If not, see <https://www.gnu.org/licenses/>.

FROM golang:1.25.5-trixie

LABEL maintainer="by-EAjks.Com <Contact@by-EAjks.Com>"

ENV DEBIAN_FRONTEND=noninteractive

ENV GOMODCACHE="/go-modules"

WORKDIR /build

RUN go mod download github.com/spf13/afero@v1.15.0 \
 && go mod download github.com/spf13/cobra@v1.10.2 \
 && go mod download github.com/spf13/viper@v1.21.0 \
 && go mod download github.com/rs/zerolog@v1.34.0 \
 && go mod download google.golang.org/grpc@v1.77.0 \
 && go mod download k8s.io/kubelet@v0.34.3
