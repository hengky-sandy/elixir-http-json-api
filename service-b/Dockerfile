FROM elixir:1.7.2

RUN mix local.hex --force
RUN mix local.rebar --force

COPY . /my_app

WORKDIR /my_app

RUN mix deps.get

EXPOSE 80

CMD mix run --no-halt