# gosexy/db/mongo

	This driver is a wrapper of [mgo](http://labix.org/mgo)

## Installation

		$ go get github.com/xiam/gosexy/db/mongo

## Usage

		import (
			"github.com/xiam/gosexy/db"
			"github.com/xiam/gosexy/db/mongo"
		)

## Connecting to a database

		sess := mongo.Session(db.DataSource{Host: "127.0.0.1"})

		err := sess.Open()
		defer sess.Close()

Read full documentation and examples on the [gosexy/db](/xiam/gosexy/tree/master/db) manual.