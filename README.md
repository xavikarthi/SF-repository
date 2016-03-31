Hello World
class Contact < ActiveRecord::Base
  self.table_name = 'salesforce.contact'
end

get "/contacts" do
  @contacts = Contact.all
  erb :index
end
