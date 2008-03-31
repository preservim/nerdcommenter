desc "Copy the vim/doc files into ~/.vim"
task :deploy_local do
  run "cp plugin/NERD_commenter.vim ~/.vim/plugin"
  run "cp doc/NERD_commenter.txt ~/.vim/doc"
end


desc "Create a zip archive for release to vim.org"
task :zip do
  abort "NERD_commenter.zip already exists, aborting" if File.exist?("NERD_commenter.zip")
  run "zip NERD_commenter.zip plugin/NERD_commenter.vim doc/NERD_commenter.txt"
end

def run(cmd)
  puts "Executing: #{cmd}"
  system cmd
end

