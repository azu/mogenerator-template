# mogenerator-template

[mogenerator](https://github.com/rentzsch/mogenerator "rentzsch/mogenerator") custom template

* add ``<$managedObjectClassName$>Object : NSObject {}``


Generator NSManagedObject & NSObject Model: 

	@interface _GizmooModel : NSManagedObject {}
	@property (nonatomic, strong) NSDate* beginDate;
	@end
	
	@interface _GizmooModelObject : NSObject {}
	@property (nonatomic, strong) NSDate* beginDate;
	@end

## Usage

Setting mogenerator ``--template-path`` options.

``--template-path /path/to/mogenerator-templates/``

e.g)

	mogenerator \
	--model $PROJECT_DIR/Model.xcdatamodeld/Model.xcdatamodel \
	--output-dir $PROJECT_DIR/App/Models/ \
	--template-path /path/to/mogenerator-templates/ \
	--template-var arc=true

See also

* [documentation - How do the Mogenerator parameters work, which can I send via Xcode? - Stack Overflow](http://stackoverflow.com/questions/3589247/how-do-the-mogenerator-parameters-work-which-can-i-send-via-xcode "documentation - How do the Mogenerator parameters work, which can I send via Xcode? - Stack Overflow")

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## License

MIT
