# grunt-allhaml

> convert each of all the haml files to html file in the directory

## Getting Started
This plugin requires Grunt `~0.4.4`

```shell
npm install grunt-allhaml --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-allhaml');
```

## The "allhaml" task


### Options

####pathRelativeTo
Type: `String`

Default value: `'./'`

####hamlcommand
Type: `String`

Default value: `'haml'`

haml command

####hamloption
Type: `String`

Default value: `'-q --no-escape-attrs'`

haml command options


####in_dir
Type: `String`

Default value: `'haml'`

Input directopry name

####out_dir
Type: `String`

Default value: `'html'`

Output directopry name

####in_ex
Type: `String`

Default value: `'haml'`

Input file extention name

####out_ex
Type: `String`

Default value: `'html'`

Output file extention name





### Usage Examples

#### Default Options
```js
grunt.initConfig({
  allhaml: {
    options: {
      in_dir: 'haml',
      out_dir: 'html',
      out_ex: 'html'
    },
    dist: {
      src: ['<%= allhaml.options.in_dir %>/**/*.haml'],
      dest: '<%= allhaml.options.out_dir %>'
    }
  },
});
```

#### Custom Options

```js
grunt.initConfig({
  allhaml: {
    options: {
      in_dir: 'haml',
      out_dir: 'html',
      out_ex: 'html',
      hamloption: ''
    },
    dist: {
      src: ['<%= allhaml.options.in_dir %>/**/*.haml'],
      dest: '<%= allhaml.options.out_dir %>'
    }
  },
});
```
