task :default => :pdf
task :pdf     => FileList["*.md"].ext("pdf")

rule ".pdf" => ".md" do |t|
  sh "pandoc -o #{t.name} #{t.source}"
end


