# LaravelBladeMinify
Minifies Laravel Blade File with HTML, CSS and JQuery on runtime.

<h2 align="left">Steps to Follow: </h2>

###

<ol>
  <ul> Create a Middleware: MinifyBlade</ul>
  <ul> Copy the Code from the php file provided. </ul>
  <ul> Register the Middleware to Kernel.php under <i>protected $middlewareAliases</i> as <br> <i> 'bladeMinify' => \App\Http\Middleware\MinifyBlade::class, </i> at the last.</ul>
  <ul> Copy all the routes under this route. as <i>Route::middleware(['bladeMinify'])->group(static function () {<br>
  });</i> </ul>
</ol>

###

