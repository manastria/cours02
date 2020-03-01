Bundler.require :default


#guard :asciidoctor
#guard :asciidoctor, :attributes => {'toc' => ''}


# Ne fonctionne pas...
#guard 'shell' do
#  watch(/^.*\.adoc$/) {|m|
#  	if m[0] != "index.adoc"
#  	Asciidoctor.render_file(m[0], :extensions=, :to_dir => "build", :safe => Asciidoctor::SafeMode::UNSAFE, :attributes=> {'sectnums'=>'','stylesheet'=>'main.css','stylesdir'=>'stylesheets/','icons' =>'font','idprefix' => '', 'idseparator' => '-', 'copycss' => '', 'source-highlighter' => 'coderay@', 'sectanchors' => '', 'doctype' => 'book', 'eruby'=>'erubis', 'toc' => 'left', 'toclevels' => '2', 'revnumber' => '1.0', 'require'=>'asciidoctor-diagram'})
#  	end
#    Asciidoctor.render_file("index.adoc", :to_dir => "build", :safe => Asciidoctor::SafeMode::UNSAFE, :attributes=> {'sectnums'=>'','stylesheet'=>'main.css','stylesdir'=>'stylesheets/','icons' =>'font','idprefix' => '', 'idseparator' => '-', 'copycss' => '', 'source-highlighter' => 'coderay@', 'sectanchors' => '', 'doctype' => 'book', 'eruby'=>'erubis','toc' => 'left', 'toclevels' => '1', 'revnumber' => '1.0', 'require'=>'asciidoctor-diagram'})
#  }
#end

guard 'shell' do
 watch(/^.*\.adoc$/) {|m|
   Asciidoctor.convert_file m[0], safe: :unsafe
 }
end

guard 'livereload' do
 watch(%r{^.+\.(css|js|html)$})
end
